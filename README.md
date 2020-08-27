# Project
LUNG SEGMENTATION


Lung segmentation is the image segmentation technique in computer vision which applies deep neural network method. From the chest X-ray, it is possible to segment the lung from the original images for medical analysis purposes.

![alt text](https://github.com/phatnguyen1190/Project/blob/master/origin.jpg?raw=true) 

![alt text](https://github.com/phatnguyen1190/Project/blob/master/lung_position.jpg?raw=true)


TEFPA framework:

    -TASK: segmenting lung's position from an X-ray image.
    
    -EXPERIENCE: X-ray images and corresponding lung's masked images dataset.
    
    -FUNCTION SPACE: model U-net. 
    
    -PERFORMANCE MEASURE: Intersection over Union (IoU) metric.
    
    -ALGORITHM: optimizer Adam.
    
HOW IT WORKS:

First, the dataset used must includes X-ray images and corresponding segmented images (black background and white object)

![alt text](https://github.com/phatnguyen1190/Project/blob/master/mask.jpg?raw=true)

For image segmentation, the job is to label Background(black) versus Object(white) for each pixel of the original image by learning through the U-net model.

![alt text](https://github.com/phatnguyen1190/Project/blob/master/u-net-architecture.png?raw=true) 

After training, Intersection over Union (IoU) metric and validation dataset loss are used to evaluate the trained model.


REFERENCES:

U-net model:  https://github.com/zhixuhao/unet

              https://github.com/bnsreenu/python_for_microscopists

Lung dataset: https://www.kaggle.com/nikhilpandey360/chest-xray-masks-and-labels

