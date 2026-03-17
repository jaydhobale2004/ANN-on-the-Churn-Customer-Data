[README_ANN_on_the_Churn_Customer_Data.md](https://github.com/user-attachments/files/26058773/README_ANN_on_the_Churn_Customer_Data.md)
# ANN on the Churn Customer Data

An **Artificial Neural Network (ANN)** project for predicting whether a bank customer is likely to stay or leave. The project uses structured tabular data and follows a complete machine learning workflow from preprocessing to evaluation.

## Overview

Customer churn prediction is a common business problem in banking and subscription-based services. This notebook builds a binary classification model using a neural network to estimate whether a customer is likely to exit the bank.

The workflow includes:

- loading the churn dataset
- preprocessing categorical and numerical features
- splitting the data into training and test sets
- scaling the features
- building an ANN using TensorFlow / Keras
- generating predictions
- evaluating the model with a confusion matrix and accuracy score

## Dataset

The notebook uses:

- `Churn_Modelling.csv`

The target variable is whether the customer exited the bank.

## Tech Stack

- **Python**
- **NumPy**
- **Pandas**
- **scikit-learn**
- **TensorFlow / Keras**
- **Jupyter Notebook / Google Colab**

## Model Architecture

The neural network is built using `tf.keras.Sequential` with:

- input features from the preprocessed churn dataset
- **2 hidden layers**
- **6 neurons per hidden layer**
- **ReLU activation** in hidden layers
- **Sigmoid activation** in the output layer for binary classification

Training configuration:

- **Optimizer:** Adam
- **Loss:** Binary Crossentropy
- **Batch size:** 32
- **Epochs:** 100

## Preprocessing Steps

The notebook includes:

- label encoding for the gender feature
- one-hot encoding for geography
- train/test split
- standard scaling for numerical consistency

## Results

The saved notebook output shows:

- **Accuracy:** 0.8605

This indicates that the model performs reasonably well for a baseline ANN on a structured churn dataset.

## Repository Contents

```text
ANN-on-the-Churn-Customer-Data/
├── Churn_Modelling.csv
└── Copy_of_ann.ipynb
```

## How to Run

1. Clone the repository.
2. Install the required dependencies:
   ```bash
   pip install numpy pandas scikit-learn tensorflow
   ```
3. Open the notebook:
   ```bash
   jupyter notebook Copy_of_ann.ipynb
   ```
4. Run the cells in order.

## Future Improvements

- tune the architecture and hyperparameters
- compare ANN performance with tree-based models such as XGBoost or Random Forest
- add ROC-AUC and precision/recall metrics
- include training curves for loss and accuracy
- refactor the notebook into a cleaner project structure with a `requirements.txt`

## Why This Project Matters

This project demonstrates:

- end-to-end supervised learning on structured data
- feature preprocessing for mixed data types
- practical deep learning with TensorFlow / Keras
- model evaluation for a business-focused classification task

## Author

**Jay Dhobale**
