## Install
**This project requires Python 3.6** 
with the pygame library installed, as well as Keras with Tensorflow backend.
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

*Make sure to install all dependencies from the included requirements.txt file as it requires specific version of packages to work properly

This will run and show the agent. The default configuration loads the file *weights/weights.hdf5* and runs a test.
The Deep neural network can be customized in the file snakeClass.py modifying the dictionary *params* in the function *define_parameters()*

## Untrained Version of AI Snake Agent
https://user-images.githubusercontent.com/11039118/148360955-cf27e96a-015b-4177-87ee-ea27437ccd2c.mp4



## Trained Version of AI Snake Agent
https://user-images.githubusercontent.com/11039118/148362370-e22a0545-385f-41c5-907c-338d4d72b905.mp4
