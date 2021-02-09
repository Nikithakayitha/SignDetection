**SIGN-LANGUAGE-DETECTOR:**

Code.ipynb
    Complete coding part for sign detection which involves:
      *Setting Paths
      *Creating Label Map
      *Creating tensorflow records
      *Downloading TF Models
      *Copying Model Configuration to Training Folder
      *Updating Configuration For Transfer Learning
      *Training the model
      *Loading Trained Model From Checkpoint
      *Detecting in Real-Time

**AIM:**

1.Labelling images for Object detection

2.Training Tensorflow for Sign language

3.Detecting Sign language in Real time

1. **Labelling images for Object detection**

Collect images using python and opencv, then label them with Lable image package

Steps:
**1. Prepare image labels using labelImg:** 
        
   Key dependencies to capture images:
    *OpenCV
    *OS: helps us work with file paths
    *Time: gives a time break in between each of the images that we collect
           (enabling to move our hands in oredr to collect different angles for the sign language model)
    *uuid: helps in naming image files
         
   Downloads required:
    *LabelImg(python package helps in labelling images for sign detection)
        Dependencies for LabelImg:
        *Install PyQt5- conda install pyqt5
        *Install lxml- conda install -c anaconda lxml
        setting up binaries- pyrcc5 -o resources.py resources.qrc
        command to run LabelImg(in cmd)- python labelling.py
    
 **2. Transfer learning using SSDMobileNet:**
 **3. Real time detection using a webcam and OpenCV:**

2.CodeToCaptureImagesWithCamera
    This code enables us to capture images which is used to train the model in recognizing the sign in real time.
