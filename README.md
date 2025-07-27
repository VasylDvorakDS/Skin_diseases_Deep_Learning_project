# Task

In this task, I need to use the UNet neural network. It is necessary to solve the problem of segmentation of dermatological lesions,
in other words moles, birthmarks, etc. The dataset contains photographs
of moles and corresponding binary masks.

Use the ISIC 3B dataset available by [full dataset](https://challenge.isic-archive.com/data),
[train dataset](https://isic-challenge-data.s3.amazonaws.com/2016/ISBI2016_ISIC_Part3B_Training_Data.zip),
link to the test [test dataset](https://isic-challenge-data.s3.amazonaws.com/2016/ISBI2016_ISIC_Part3B_Test_Data.zip) (the data takes about 800mb).
Prepare this data for training, select an optimizer and its hyperparameters, train your model on the training data, and also
evaluate the quality of this model on the test sample.


<img width="940" height="851" alt="изображение" src="https://github.com/user-attachments/assets/5ed5800a-e075-4921-ac89-b52712bcd83a" />


# Output

The UNet model showed a low IoU=0.3372 metric. This is due to the fact that the images contain artifacts from the doctor's monocle. 
It is necessary to create an algorithm for their automatic pruning or apply the simplest algorithm for detecting moles, and then segmentation.
