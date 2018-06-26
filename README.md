# LaneDetection
Lane Detection for Autonomous Driving Using Deep Learning

This code uses real world dataset CanVid dataset from Cambridge University for training and testing. Images are collection of street views obtained while driving. The dataset contains pixel to pixel labels.

The main idea of semantic segmentation using deep learning is to do away with computer vision techniquies since it has issues like image resolution, camera calibration,etc

Semantic segmentaion refers to complete scene understanding and dividing image into various segments one such segment which is of our use is the road or lane and vehicle. 


The data is split into 60/40 ratio for training and testing. We are using pretrained Segnet for semantic segentation. Since the training takes time and was intitially trained by mathworks on Nvidia TitanX which took approximately 5 hours. 
We used this pretrained network and narrowed down the classes from 30 to 2 i.e road and pedestrian.

While grouping two or more classes similar classes get grouped together like
Car={Car, Truck, SUV, Moving Vehicle}

SegNet is initialised with weigths of pretrained VGG16.

We also downsize the images to reduce the training time.

Since there are unequal instances of each class in dataset we balance classes using class weighting.

Feel free to contribute and extend the scope to the project:)


