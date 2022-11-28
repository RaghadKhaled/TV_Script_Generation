# Generate TV script using Embeddings and LSTM

--- 

## Overview

In this project, I worked to addressing the problem of generating a new Seinfeld TV scripts using RNNs.  Given a word, the RNN model will automatically predict the most likely next word. In order to generate a text of words, firstly we need to determine the start word and specific length of words to repeat the prediction. Then, we will obtain a text which represent a new “fake” TV script. I did this project as a part of Deep Learning Nanodegree from Udacity.
I did this project as a part of Deep Learning Nanodegree from Udacity. 

--- 

## Dataset

The data is a subset of Seinfeld TV dataset of scripts from 9 seasons. 
You can find more information for the full dataset [on Kaggle](https://www.kaggle.com/datasets/thec03u5/seinfeld-chronicles).

--- 


## Project Steps

The high-level steps of the project include:
1.	Preprocessing of dataset (include lookup table, tokenization)
2.	Prepare the batches
3.	Build the RNN network. It consists of embedding layer, LSTM layer and fully connected layer.
4.	Training and testing.
5.	Create TV script generation algorithm – this algorithm takes the model I created, start word, length of text to generate new text.

--- 

## Results

I test the model with ```jerry``` as start word and 400 total length of text , the results are showed below. 

```
jerry:!(waves the keys from jerry)

jerry: oh.

elaine:(to kramer) you know, i got a problem with the woman.

jerry:(to elaine) what?

george: i don't want to know that.

jerry: what is wrong with you, that is so bad.

george: what are you doing here, jerry, you know? you know, i have no idea how to have sex with the guy....

jerry: oh! yeah, you know, i think i'm gonna get out of here.

george:(to george) you know, you know, i think i could get you a little more enthusiastic...

george:(pointing to the counter) oh, hi, jerry.

george: what about my last date?!

kramer:(shouts) i don't think you can take a bite!

jerry: i thought you said that.

jerry: i thought you were going to be a lot of a good time, i don't have any trouble. i was a little bit of the commercial.

kramer: yeah, i know.

jerry:(to jerry) i don't know. i mean, if you could just do it.

george:(sarcastic) i thought he was a kid. i can't do this!

george:(to george) hey, what are you doing?

george: i think i can. i just don't think we have a good thing.

kramer: well, i don't know what to do.

george: well, if we should just get a little tired of that.

jerry: oh, i don't think so. i think it's a good idea. i mean, i have to go to the bathroom.

jerry: i don't know why you can't do it.

kramer: i don't think so.

george: i don't think so.

elaine: oh.... no. no, no no no
```



---

## Requirements	
- Python 3.7
- Numpy 
- Torch
- Jupyter Notebook
- Maybe needs to use GPU


---

## Running the project
The whole project is located in the jupyter notebook file ``` dlnd_tv_script_generation ```, you can use the Anaconda environment to open the Jupyter Notebook and install the requirement.
