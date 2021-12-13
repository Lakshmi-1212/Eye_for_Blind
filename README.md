# EYE FOR THE BLIND - generating captions for images

## Overview
The World Health Organization (WHO) has reported that approximately 285 million people are visually impaired worldwide, and out of these 285 million, 39 million are completely blind. It gets extremely tough for them to carry out daily activities, one of which is reading. From reading a newspaper or a magazine to reading an important text message from your bank, it is tough for them to read the text written in it.

A similar problem they also face is seeing and enjoying the beauty of pictures and images. Today, in the world of social media, millions of images are uploaded daily. Some of them are about your friends and family, while some of them are about nature and its beauty. Understanding what is present in that image is quite a challenge for certain people who are suffering from visual impairment or who are blind.

In an initiative to help them experience the beauty of the images, Facebook had earlier launched a unique feature earlier that can help blind people operate the app on their mobile phones. The feature could explain the contents of an image that their friends have posted on Facebook. So, say, if someone posted a picture with their dog in the park, the application would speak out the contents and may describe it like, “This image may contain a dog standing with a man around the trees.”

## Problem Statement
In this capstone project, you need to create a deep learning model which can explain the contents of an image in the form of speech through caption generation with an attention mechanism on Flickr8K dataset. This kind of model is a use-case for blind people so that they can understand any image with the help of speech. The caption generated through a CNN-RNN model will be converted to speech using a text to speech library.

This problem statement is an application of both deep learning and natural language processing. The features of an image will be extracted by a CNN-based encoder and this will be decoded by an RNN model.

The project is an extended application of Show, Attend and Tell: Neural Image Caption Generation with Visual Attention paper.

The dataset is taken from the Kaggle website and it consists of sentence-based image descriptions having a list of 8,000 images that are each paired with five different captions which provide clear descriptions of the salient entities and events of the image.

In this project, you will convert an image to text description first; then, using a simple text-to-speech API, you will extract the text description/caption and convert it to audio.   

## Major Steps
- Data Understanding: Here, you need to load the data and understand the representation.
- Data Preprocessing: In this step, you will process both images and captions to the desired format.
- Train-Test Split: Combine both images and captions to create the train and test dataset.
- Model Building: This is the stage where you will create your image captioning model by building Encoder, Attention and Decoder model.
- Model Evaluation: Evaluate the models using greedy search and BLEU score.