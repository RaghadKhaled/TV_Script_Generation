# Generate TV script using Embeddings and LSTM

--- 

## Overview

In this project, I worked to addressing the problem of generating a new Seinfeld TV scripts using RNNs.  Given a word, the RNN model will automatically predict the most likely next word. In order to generate a text of words, firstly we need to determine the start word and specific length of words to repeat the prediction. Then, we will obtain a text which represent a new “fake” TV script. I did this project as a part of Deep Learning Nanodegree from Udacity.
I did this project as a part of Deep Learning Nanodegree from Udacity. 

--- 

## Dataset

The landmark images are a subset of the Google Landmarks Dataset v2. It has different 50 landmarks from all of the world. You can download the datatset by [this link](https://udacity-dlnfd.s3-us-west-1.amazonaws.com/datasets/landmark_images.zip). You can find more information for the full dataset [on Kaggle](https://www.kaggle.com/google/google-landmarks-dataset).

--- 


## Project Steps

The high-level steps of the project include:
1.	Build a CNN to Classify Landmarks (from Scratch) 
2.	Build a CNN to Classify Landmarks (using Transfer Learning)  – I used VGG16 since my dataset has similar feature of the dataset that trained on the VGG16. Therefore, most or all of the pre-trained neural network layers already contain relevant information about the my dataset. I Use all but the last fully connected layer as a fixed feature extractor and I define a new, final classification layer to match the number of classes of my task. I randomize the weights of the new fully connected layer and freeze all the weights from the pre-trained network then I train the network to update the weights of the new fully connected layer.
3.	Create Landmark Prediction Algorithm – this algorithm take the best model I created to make interface for any user-supplied image as input and suggest the top k most relevant landmarks from 50 possible landmarks from across the world. 
All the implementation details are in jupyter notebook file ``` landmark.ipynb```.

--- 

## Results

I test the model from image in my computer, the results are showed below. 

<div align="center">
<p>
<img src="Untitled - Frame 1.jpg" width="400" height="800"/>
</p>
<br>
<div>
</div>
</div>



---

## Requirements	
- Python 3.7
- Numpy 
- Torch
- Torchvision
- PIL
- OpenCV
- Matplotlib 
- Jupyter Notebook
- Maybe needs to use GPU


---

## Running the project
The whole project is located in the jupyter notebook file ``` landmark.ipynb ```, you can use the Anaconda environment to open the Jupyter Notebook and install the requirement.
