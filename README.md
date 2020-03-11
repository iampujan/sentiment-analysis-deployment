# sentiment-analysis-deployment

This project is a final project of Udacity Deep Learning Nanodegree.
Deployment is done using Amazon Sagemaker.

Creating a Sentiment Analysis Web App
Using PyTorch and SageMaker
Deep Learning Nanodegree Program | Deployment

Now that we have a basic understanding of how SageMaker works we will try to use it to construct a complete project from end to end. Our goal will be to have a simple web page which a user can use to enter a movie review. The web page will then send the review off to our deployed model which will predict the sentiment of the entered review.


General Outline
Recall the general outline for SageMaker projects using a notebook instance.

1. Download or otherwise retrieve the data.
2. Process / Prepare the data.
3. Upload the processed data to S3.
4. Train a chosen model.
5. Test the trained model (typically using a batch transform job).
6. Deploy the trained model.
7. Use the deployed model.
For this project, you will be following the steps in the general outline with some modifications.

First, we will not be testing the model in its own step. We will still be testing the model, however, we will do it by deploying our model and then using the deployed model by sending the test data to it. One of the reasons for doing this is so that we can be sure that our deployed model is working correctly before moving forward.

In addition, you will deploy and use your trained model a second time. In the second iteration we will customize the way that our trained model is deployed by including some of our own code. In addition, our newly deployed model will be used in the sentiment analysis web app.
