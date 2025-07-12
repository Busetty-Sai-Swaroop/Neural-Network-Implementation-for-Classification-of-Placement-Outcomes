
# Neural Network Implementation for Classification of Placement Outcomes

## Problem Statement
Predicting student placement based on academic and interview performance using a Feed-Forward Neural Network (FNN). The model uses features like GPA, interview score, and skills score to determine the probability of placement.

## Description
This project focuses on predicting whether a student will be placed based on several academic and skill-related factors. The prediction model is built using a Feed-Forward Neural Network (FNN) trained on historical data to recognize patterns in student performance. The system helps students and institutions assess placement probabilities by leveraging Supervised Learning.

## What is a Neural Network?
A Neural Network (NN) is a computational model inspired by the human brain. It consists of interconnected neurons (nodes) that process input data and generate outputs. These networks identify patterns, make predictions, and solve complex problems by mimicking how the brain learns.

### Feed-Forward Mechanism
A Feed-Forward Neural Network works by:
1. Taking input features (GPA, interview, and skills scores).
2. Passing them through multiple hidden layers with activation functions like ReLU (Rectified Linear Unit).
3. Producing an output layer with a sigmoid activation function to classify the result.

## Objective
To develop a Neural Network Model that predicts whether a student will be placed based on their GPA, interview score, and skills score.

## Factors Affecting Student Placement
- GPA (0-10 scale)
- Interview Score (0-100)
- Skills Score (0-100)
- Placement Status (Label: 0 for Not Placed, 1 for Placed)

## Algorithm for Neural Network Implementation
1. Load Dataset: Read student placement data from a CSV file.
2. Preprocess Data: Normalize feature values between 0 and 1.
3. Split Dataset: Divide the dataset into 80% training and 20% testing sets.
4. Build Neural Network:
    - Input Layer: 4 nodes (GPA, Work Experience, Interview Score, Skills Score).
    - Hidden Layers: 2 layers with ReLU activation.
    - Output Layer: 1 node with Sigmoid activation.
5. Compile Model: Use Adam optimizer and binary cross-entropy loss function.
6. Train Model: Fit the model using training data with 200 epochs.
7. Evaluate Performance: Measure accuracy on the test dataset.
8. Predict Outcome: Classify user input as Placed or Not Placed.

## Data Preprocessing
- The dataset is loaded from a CSV file, extracting relevant features (GPA, Work Experience, Interview Score, Skills Score).
- The data is normalized by scaling values between 0 and 1 to improve model performance.

## Neural Network Architecture
- The input layer consists of 4 nodes (one for each feature).
- Two hidden layers with ReLU activation enhance the network’s ability to learn complex patterns.
- The output layer has one node with a sigmoid activation function, classifying whether the student will be placed (1) or not (0).

## Model Training
- The dataset is split into 80% training and 20% testing.
- The Adam optimizer is used for model optimization, and binary cross-entropy loss measures classification accuracy.
- The model is trained over 200 epochs to improve its generalization ability.

## Prediction and Evaluation
- After training, the model evaluates performance using the test dataset.
- A probability score is generated for each student's data, classifying them as either Placed (1) or Not Placed (0) based on a 0.5 threshold.

## Conclusion
This project successfully developed a Feed-Forward Neural Network (FNN) to predict student placement based on academic and skill-related factors. The model achieved high accuracy in predictions by normalizing features, training on real-world data, and optimizing the neural network architecture. The system provides real-time placement probability estimates, helping students and institutions analyze strengths and weaknesses for better job preparation.
