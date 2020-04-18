## Running The Code

To run any of the provided programs:

* Upload the file to Google Colab.
* Enable GPU on Google Colab.
* Change the folder variable (located in cell 4 underneath the imports). This folder variable should contain the path to the folder where you want data to be saved. The folder in the path should NOT exists, otherwise the program will expect certain files to be in there, like parameters to load in the model.
* If you want to view the Tensorboard, set the logdir flag (located in the last cell) to be the same as the folder variable.  
* Run all the cells (if you do **NOT** want to mount your Google Drive; delete the second cell, then run all the cells). 

## What The Code Does

During training, the program will:

* Load parameters from the folder if any exists.
* Train the model and track the time it takes.
* Save Tensorboard data.
* Periodically save parameters.

After training, the program will:

* Save the best model.
* Save NumPy plotting data.
* Test the trained model and save the predictions to a file.
* Plot the data from training.

