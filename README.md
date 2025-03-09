# Major-Project
Final year major project

## Dataset used -> UCF crime dataset 
google drive link to which will soon be given.

## Steps to run:
* Download the video dataset, it might be long as it contains large video files
* Clone the repo
* Make a seperate subfolder inside the cloned project folder for the dataset and name it "UCF" as used in the codebase
* Run the videodata file to extract frames from the videos
* Finally run the main file that will be responsible for the preprocessing, training and storing the model.

## Highlights
* Got an accuracy of  above 99 percent with the LSTM model
* Performance metrics show that the model works really well on the unseen data

### Information on the **Model** used
For this project, I implemented and evaluated two different machine learning models:

1️ Support Vector Machine (SVM)
Model: SVC(kernel='linear') (Support Vector Classifier with a linear kernel)
Purpose: Used for classification tasks on structured data
Training: Trained on X_train, y_train and tested on X_test, y_test
Performance Metric: 99.98 %
2️ Multi-Layer Perceptron (MLP)
Model: A deep learning model built using Keras' Sequential API
Architecture:
Dense(512, activation='relu') (Input Layer)
Dropout(0.5) (Regularization)
Dense(256, activation='relu') (Hidden Layer)
Dropout(0.3)
Dense(len(set(labels)), activation='softmax') (Output Layer for multi-class classification)
Compilation:
Loss Function: sparse_categorical_crossentropy
Optimizer: adam
Both models were compared based on their accuracy to determine the best-performing approach for the given dataset and actually, both worked very well giving above 99 percent accuracy.

