# Pneumonia Detection.

## Description: 

This project focuses on developing a pneumonia detection model using machine learning techniques. The project is structured into several steps.

In the initial part, the code imports necessary libraries, including "mahotas" for image processing and the "RandomForestClassifier" from scikit-learn for the machine learning model. It also ensures the installation of the required "mahotas" library.

The code then proceeds to download and extract a subset of the Kaggle Pneumonia Dataset. The dataset consists of chest X-ray images classified as normal or pneumonia. The images are organized into two directories: "normal/" and "pneumonia/".

Following the dataset acquisition, the code performs data wrangling operations. It reads the images, converts them to grayscale, resizes them to a uniform size of (300 x 300) pixels, and stores the pixel values in numpy arrays named "normal_images" and "pneumonia_images". Each array corresponds to a specific class, normal or pneumonia.

After the data wrangling, the code displays the first 5 images from both the normal and pneumonia classes using matplotlib's ImageGrid.

To train and evaluate the machine learning model, the code creates a balanced dataset. It selects 60 images from each class for training and 40 images from each class for testing. The images are flattened into one-dimensional arrays and stored in the "training_data" and "testing_data" arrays, respectively. The corresponding labels (0 for normal, 1 for pneumonia) are stored in the "training_target" and "testing_target" arrays.

A Random Forest classifier is then initialized using scikit-learn's RandomForestClassifier. The model is trained on the training data and labels using the fit() function.

Next, the model's accuracy is evaluated by predicting the labels for the testing data using the predict() function. The classification accuracy is calculated using the score() function. Additionally, the code computes and displays the confusion matrix and accuracy score using scikit-learn's confusion_matrix() and accuracy_score() functions.

Overall, this project aims to develop a pneumonia detection model using machine learning. The code imports necessary libraries, processes the dataset, trains a Random Forest classifier, and evaluates its accuracy. The project provides insights into potential improvements and highlights misclassified images for further analysis.


### Programing Language: 
1. Python

### Libraries:
1. Numpy
2. Pandas
3. os
4. Matplotlib
5. mahotas
6. sklearn
