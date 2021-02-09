# SIGN-LANGUAGE-DETECTION:

## Code.ipynb

   ### Sign detection code consists of:
   
   *Set up Paths
    
   *Label Map
    
   *Tensorflow records
   
   *TF Models
   
   *Transfer Learning Configuration
   
   *Model training
   
   *Detection in Real-Time

## Worked on:

1.Labelling images for Object detection

2.Training Tensorflow for Sign language

3.Detecting Sign language in Real time

### Collecting images:
        
   Key dependencies to capture images:
   
   #### OpenCV: 
   Enables the image and video processing to identify objects, faces, or even handwriting of an human.
   
   #### OS: 
   helps us work with file paths
   
   #### Time: 
   gives a time break in between each of the images that we collect(enables to collect different angles)
   
   #### uuid: 
   helps in naming image files

Create a folder to save the images captured using the IMAGES_PATH. Next thing is to create labels that we are going to collect and specifying the number of images required. Later on, create a directory for labels, and start collecting images using the video capture. Finally, on collecting images, we have to get all the images to a single folder in order to label them with no duplications.
         
### Setup LabelImg(python package helps in labelling images for sign detection)
        
   Dependencies for LabelImg:
        
   **Install PyQt5** conda install pyqt5
        
   **Install lxml** conda install -c anaconda lxml
    
These commands enables label image work properly:

   **setting up binaries** pyrcc5 -o resources.py resources.qrc
   
   
### Label Image and create Labelmap

**command to run LabelImg** python labelling.py
Specifically, we need to label each one of sign language poses. To do that, we have to use the labelling tool to draw square around the pose and type in the name of the label. Now on labelling data, we have to split them up into a training and testing partitions, which allows our model to train on a certain set of data, and test and evaluate on a seperate partition.

Label map is a representation of all the different objects that we got within the model. After creating the labelmap, we have to go with tf records, which is a special file format the tensorflow object detection api likes to be trained.

### Training model and detection

Dependencies dor training model:

label_map_util and visualization_utils from object_detection.utils

model_builder from object_detection.builders
   
Successful model building enables us to make real-time detections.

**Not just Sign detection we can even work on different posture detection in a similar way.**
