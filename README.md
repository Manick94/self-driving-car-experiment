# Self Driving Car Experiment
## Author: (EJ) Vivek Pandey
### The VR environment involved in the training/test has not been committed due to the huge file sizes and my git lfs is full lol

## Dependencies
You need to have anaconda in your system first.

# TensorFlow without GPU
`conda env create -f environments.yml`

# TensorFlow with GPU
`conda env create -f environment-gpu.yml`

# To activate the environment
`source activate self-driving-car-env`

# To see how it works
* Clone this repo, duh!
* Get the VR env from Udacity's repo - the binary works out-of-the-box: https://github.com/udacity/self-driving-car-sim
* Launch the VR env in training mode
* Start the recording, provide a location to store the frames, and drive a minimum of 5-7 laps
* Train the model by running `python model.py` (Check out the arguments in the file and provide as necessary, especially the location for training images)
* Should take about 8-9 hours if you have a fairly powerful system and your training is based off of only a few laps, or else run it in a GPU instance
* If the training time scares you and you choose to use the pretrained model, feel free to skip the training steps above.
* Launch the VR env in autonomous mode
* Kick off the driver using `python drive.py "model.h5" "folder_to_save_images_to"`
* Watch the magic happen