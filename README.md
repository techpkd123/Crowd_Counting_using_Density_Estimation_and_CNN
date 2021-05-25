# Crowd_Counting_using_Density_Estimation_and_CNN
## Context
The problem of object counting is a difficult problem in which you have an image and have to count all the certain objects on that image, this becomes intractable in the context of big data and internet of things when you have videos tracking and need to count the objects in every frame. This problem can be achieved by an automatic process like a machine learning algorithm that receives a image as input and gives the number of some object of interest in the image (discrete value). For that different approaches can be done, the typical and easier is consider the number of element in the image as a label and transform it to some classification problem, other transform to a regression problem and other ones use a fully convolutional architecture in where the final convolutional output can be consider the numbers of object in that region and then sum up.


## Dataset(few files not avalilable in the repo because of the big size of the dataset but nevertheless I have properly commented the code along with markdowns in notebook)
The dataset is composed by RGB images of frames in a video (as inputs) and the object counting on every frame, this is the number of pedestrians (object) in the image. The images are 480x640 pixels at 3 channels of the same spot recorded by a webcam in a mall but it has different number of person on every frame, is a problem of crowd counting.

![image](https://user-images.githubusercontent.com/49801313/119560829-0e878680-bdc2-11eb-8c57-deb43d5da22d.png)
 


We give the images data as a binary file of NumPy (.npy format) that you can easily load with the numpy load function. If you want to load image by image we also give the JPG images in a folder.

The labels/target are the number of person on the frame JPG image and there is one for each image. This are integer numbers of the counting, for example in the Image above there are 29 objects (people).

![image](https://user-images.githubusercontent.com/49801313/119560850-1515fe00-bdc2-11eb-9b6b-26358b70edca.png)

## Installation Instructions

#### Make sure you have all the dependencies installed like:-

   Tensorflow(Latest version)if not using
    
    -pip install tensorflow
    
   Then Clone the Repo using
      
     -git clone https://github.com/techpkd123/Crowd_Counting_using_Density_Estimation_and_CNN.git
    
   Then you are good to go and can explore the project(i.e. notebook)
    

## Reference and Motivation.
https://www.analyticsvidhya.com/blog/2019/02/building-crowd-counting-model-python/

 
