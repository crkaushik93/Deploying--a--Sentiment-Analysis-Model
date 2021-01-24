# Deploying--a--Sentiment-Analysis-Model

# Project Overview

Welcome to the SageMaker deployment project! In this project you will construct a recurrent neural network for the purpose of determining the sentiment 
of a movie review using the IMDB data set. 
You will create this model using Amazon's SageMaker service. In addition, you will deploy your model and construct a simple web app which will interact with the deployed model.

identified key details in the pre-processing method. Here are all the 5 steps:

Get text only out of the input review by removing html format (if any).
Lower the text and then replace the pattern specified with space, that is, replace all characters that are not alphabets nor digits with space.
Split each word of the text into a list (separated by a space).
Remove all stopwords in the list.
Stemming each word in the list. (convert entitled/entitling -> entitl, builds/building -> build, ...)

The build_dict method is implemented and constructs a valid word dictionary.

The train method is implemented and can be used to train the PyTorch model.

The RNN is trained using SageMaker's supported PyTorch functionality.

The trained PyTorch model is successfully deployed.

The test review has been processed correctly and stored in the test_data variable.

describes the differences between the RNN model and the XGBoost model and how they perform on the IMDB data.

The predict_fn() method in serve/predict.py has been implemented.

The model is deployed and the Lambda / API Gateway integration is complete so that the web app works (make sure to include your modified index.html).

