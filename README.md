# Autism-Detection-In-children-Using-Facial-Images
Our aim is to develop a binary classifier  for discriminating the two classes of  facial image . We have to train  the classifier that can predict the class of participants into autistic (1) and non-autistic (0) using CNN classifier of machine learning .

## Dataset Description- 

1. Dataset (Name/ Description) - Learning to predict autism spectrum disorder based on the facial image
2. Characteristics of dataset - This dataset includes visualizations of facial image with a particular focus Autism Spectrum Disorder (ASD).
3. URL - https://www.kaggle.com/gpiosenka/autistic-children-data-set-traintestvalidate



## Methodology 
1.  Load Train dataset:  First, we will start by training our dataset. Our dataset contains the file with file names as “Non_Autistic.135.jpg , Autistic.391.jpg”, where the word is splitted by ‘.’, initial word describes the kind (whether the person is autistic or not and next word describes the image no.).

2. Load Test dataset: Our dataset contains the file with file names as “Non_Autistic.135.jpg , Autistic.391.jpg”
3.  We will be using Multi layer neural networks as deep neural networks.
4.  Since the dataset consists of images ,Convolutional neural networks will be used.
The CNN classification is a technique to segregate the data according to different categories. Each time an image is passed, it will go through a number of convolutional layers and filters.
5. Preparing Model: Then, we will prepare the model following the steps given below:
6. We will define hyperparameters
7. Then Flatten the output layer to 1 dimension
8. Further we will add a fully connected layer with 512 hidden units and ReLU activation
9. Next a dropout rate of 0.5 will be added
10. Lastly a final sigmoid layer for classification will be added
11. Preprocessing of Data: We will be preprocessing the data and extracting data from images in the form of matrix.
12. Preparing the training dataset: 
  *  Training Generator: Here we will be preparing and generating the train data.
  *  Validation Generator: We will be creating a validation generator to filter out the data to ensure the quality of performance by using the validate data.
  *  validation_data: Data on which to evaluate the loss and any model metrics at the end of each epoch. The model will not be trained on this data. 
13. Model Fitting: Now we will train the data for a fixed number of epochs and batch size.
14. Preparing the testing dataset: We will create a testing generator for generating the test dataset using the previously loaded test images.
15. Prediction: Now, we will be predicting the result for the test dataset and using the model evaluated earlier.

17. Output will be as follows : 
Image name as :- actual_name(image name{0 or 1}) , eg. autistic.127.jpg(1) , here 0/1 is prediction.
17. Our predictions will next go to submission_13010030.csv. 
This file contains the predicted result, and further we will calculate its accuracy , precision etc. 

## Results
* Number of images which were classified as :
  *  predicted Autistic :  167
  * predicted Non Autistic :  133
  * Actual Autistic :  150
  * Actual Non Autistic :  150
* Percentage of images classified as :
  * Actual Non Autistic percentage in total test data:  50.0 %
  * Predicted Non Autistic percentage in total test data:  44.333333333333336 %
  * Actual Autistic percentage in total test data:  50.0 %
  * Predicted Autistic percentage in total test data:  55.666666666666664 %
* Confusion matrix was used for predicting accuracy & other results:
  * True positive :  135
  * True Negative :  118
  * false Positive :  15
  * false Negative :  32
* Accuracy is:  84.33333333333334 %
* Precision is:  90.0 %
* Sensitivity is:  80.83832335329342 %
* Specificity is:  88.7218045112782 %

Demo Video : https://drive.google.com/file/d/1KLa4vEWLMmOdit_h9RmTulsF5Nzr4MVh/view?usp=sharing
