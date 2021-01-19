## udacity-aws-sagemaker

Project **Deploy a Sentiment Analysis Model** for Udacity Machine Learning Nanodegree

This repo contains the files that were edited/modified for the submission of the aforementioned project:

1. notebook: How the data was processed, split and transformed to numerical representations. How the model (and its artifacts) was built, tested and deployed to a Sagemaker endpoint. How the web app (client) accesses the deployed endpoint through AWS Lambda and API Gateway services. Given the right permissions, the lambda function is triggered when user submits a text for analysis and the code is executed. API Gateway provides a new endpoint that acts as an interface between the function and the web app.
2. `train/train.py`: how the model's training parameters are implemented. This file is picked up by the model object defined in the notebook and its parameters are sent as arguments when the script is executed.
3. `serve/predict.py`: how the model performs inference and computes the result when called with new data.
4. `website/index.html`: Basic html structure to call the API endpoint, invoke the Lambda function and return what the function indicates.

