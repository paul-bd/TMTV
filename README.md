# TMTV
Here is how to perform the inference for the different folds of [Fully automatic segmentation of diffuse large B cell lymphoma lesions on 3D FDG-PET/CT for total metabolic tumour volume prediction using a convolutional neural network.](https://doi.org/10.1007/s00259-020-05080-7).

# Usage
## Install the required libraries : 
You will first need and assure that the [nnunet library is correctly working](https://github.com/MIC-DKFZ/nnUNet) and configure required paths.

## Download weights : 
Weights can be downloaded at the following [link](https://www.dropbox.com/sh/pxuizooogf01ywp/AAAMQq_X0pPVU1X0DE9mBmAba?dl=0)

## to perform inference
In the PATH_FOLDER every patients should be numbered as patientID_0000 for CT and patientID_0001 for PET in the nifti format wheree CT should be in hounsfield unit and PET in SUV.

Then from the terminal type:

nnUNet_predict -i PATH_FOLDER -o ./PATH_OUTPUT -t 1


