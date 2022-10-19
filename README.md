# Semi-supervised-labeling-of-training-data
Label the rare objects in autonomous driving scenario
This work is intended to develop a pipeline to help the research community in minimalizing the manual efforts in labeling the objects, specifically focused on rare objects found in the context of autonomous driving. Though there are a lot of advancement in the field of computer vision, the manual labeling of images to train the model is a cumbersome work especially for custom dataset.Towards this goal, this work implements various object localization algorithm and test their performance on various datasets for different object of interest.Various problems were encountered during analysis which hinders the implementation in practical scenario. Further research is needed for avoiding false positives as they are critical for the objective.

The code named 'Code_to _crop_objects_from_KITTI_dataset' crops the images from KITTI dataset for specific objects as required for this project

The initial interest of the work was to identify the images from input dataset which have the object of interest.The following 2 codes are employed to implement the 2 different models developed.

The code 'Siamese_model' implements the Siamese neural network for identifying similar objects from the test dataset.
The code 'Transfer_Learning_mobilenet_with_sliding_window' classifies the specific object of interest from test dataset.

Later the focus of the study was to localize the identified object.The following codes are employed to implement mobilenet SSD or EfficientDet D0 model for identifying the rare object of interest from the large input dataset.

The code '1.Object_Localization-Labelling' is used to label the the training data with specific object.
The code '2.Object _Localization_MobilenetSSD_and_Efficientdet' is used for training and testing the specific rare object of interest.
