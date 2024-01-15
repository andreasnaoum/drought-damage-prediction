# Deep Learning for Drought Damage Prediction Using Smartphone Images of Crops

## CNN Model Results
| Model              | RMSE         |
| ------------------ | ------------ |
| CNN                | 16.44817351  |
| CNN with Heuristic | 15.69013985  |

The results were measured in the Zindi Platform, and the competition can be found here: 
https://zindi.africa/competitions/cgiar-eyes-on-the-ground-challenge

## Data Sources 
The project exclusively uses data from the "Eyes on the Ground" Challenge, consisting of 26,068 labeled training images and 8,663 testing images. The dataset was contributed by smallholder farmers making insurance claims.

## Data Analysis and Preprocessing
The methodology includes an analysis of the dataset to extract insights, preprocessing techniques such as image resizing and normalization, and the transformation of categorical data. Training, validation, and test sets were created for model development.

## Convolutional Neural Network
A CNN architecture, inspired by successful image processing tasks, was implemented using TensorFlow. The network is trained to predict the percentage of drought damage in processed images. Model assessment is based on the Root Mean Squared Error (RMSE) metric.

## Heuristic 
In this project, a CNN is combined with a heuristic to enhance model predictions. The heuristic chosen for this study combines the two most prominent choices in the survey results, namely yellow and brown leaves. In order to detect these leaves in the dataset's images, it opted to utilize a colour mask which filters pixel colours in a range between two RGB values chosen to approximate the colours of yellow and brown leaves. This colour transformation was performed during the pre-processing stage of the training, after the resizing and padding of the images.


