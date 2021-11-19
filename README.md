## Install
This project requires Python 3.6 with the pygame library installed, as well as Keras with Tensorflow backend.
```bash
git clone git@github.com:atvjoey/cs301AIgame.git
```

## Run
```python
python snakeClass.py --display=True --speed=50
```
Arguments description:

- --display - Type bool
- --speed - Type integer

This will run and show the agent. The default configuration loads the file *weights/weights.hdf5* and runs a test.
The Deep neural network can be customized in the file snakeClass.py modifying the dictionary *params* in the function *define_parameters()*

To train the agent, set in the file snakeClass.py:
- params['load_weights'] = False
- params['train'] = True

In snakeClass.py you can set argument *--display*=False and *--speed*=0, if you do not want to see the game running. This speeds up the training phase.

## For Mac users
It seems there is a OSX specific problem, since many users cannot see the game running.
To fix this problem, in update_screen(), add this line.

```                              
def update_screen():
    pygame.display.update() <br>
    pygame.event.get() # <--- Add this line ###
```
