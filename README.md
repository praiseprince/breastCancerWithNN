# Breast Cancer Classification using Neural Network

## About the Project

This project demonstrates the use of a neural network for classifying breast cancer tumors as benign or malignant. The dataset used in this project is the Breast Cancer Wisconsin (Diagnostic) Data Set, which is available at [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)). The goal of this project is to build a model that can accurately classify breast cancer tumors based on their features.

## Code Explanation

- **Data Collection and Processing**: The breast cancer dataset is loaded from sklearn and converted into a pandas DataFrame. The dataset contains 30 features and a target variable indicating the class label (0 for benign and 1 for malignant).

- **Data Preprocessing**: The data is split into training and testing sets using `train_test_split` function from sklearn. The features are then standardized using `StandardScaler` to ensure all features have a mean of 0 and a standard deviation of 1.

- **Building the Neural Network**: The neural network model is built using Keras Sequential API. It consists of an input layer, a hidden layer with 20 neurons and ReLU activation function, and an output layer with 2 neurons and sigmoid activation function. The model is compiled with the Adam optimizer and sparse categorical crossentropy loss function.

- **Training the Neural Network**: The model is trained on the training data with a validation split of 0.1 and for 10 epochs. The training process is visualized using matplotlib to show the model's accuracy and loss on both training and validation data.

- **Model Evaluation**: The trained model is evaluated on the test data, achieving an accuracy of approximately 97%. The model's predictions are then compared with the actual labels to evaluate its performance.

- **Predictive System**: A simple predictive system is implemented to demonstrate how the trained model can be used to make predictions on new data. The input data is standardized before making predictions.

## Files

- `breastCancerWithNN.ipynb`: Jupyter notebook containing the code for data preprocessing, model building, training, and evaluation.
- `dataset.txt`: Text file containing the link to the dataset used in the project.
- `model/breastCancerNN.h5`: Saved model file containing the trained neural network for breast cancer classification.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/breast-cancer-classification.git
