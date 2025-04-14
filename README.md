# IML_Project
ML Final Project: Traffic Congestion Level Prediction

This project is aimed at predicting traffic congestion levels (Low, Medium, High) using machine learning techniques. The project uses a Random Forest Classifier with One-vs-Rest strategy and includes data preprocessing, balancing with SMOTE, and evaluation metrics.

Project Structure

.
├── train.py              # Script to train the model
├── test.py               # Script to test the model
├── data_cleaned.csv      # Cleaned dataset
├── model.joblib          # Saved trained model (generated after running train.py)
├── scaler.joblib         # Saved scaler for preprocessing (generated after running train.py)
├── label_encoder.joblib  # Saved label encoder for target classes (generated after running train.py)
├── requirements.txt      # Python dependencies (optional)
└── README.md             # Project documentation (this file)

Requirements

Python 3.x

Install the dependencies using pip:

pip install -r requirements.txt

If you don't have a requirements.txt, you can install manually:

pip install pandas numpy scikit-learn imbalanced-learn joblib

Files Description

train.py

Loads and preprocesses the data.

Encodes categorical features and the target variable.

Applies SMOTE to balance the dataset.

Scales features using StandardScaler.

Trains a RandomForest classifier wrapped in One-vs-Rest.

Saves the trained model, scaler, and label encoder for future use.

test.py

Loads the saved model, scaler, and label encoder.

Prepares the test dataset.

Performs predictions on the test data.

Outputs evaluation metrics including accuracy, precision, recall, F1 score, classification report, and confusion matrix.

How to Run

Step 1: Train the model

Run the following command to train the model and save necessary artifacts:

python train.py

After successful execution, it will generate:

model.joblib

scaler.joblib

label_encoder.joblib

Step 2: Test the model

Run the following command to evaluate the trained model:

python test.py

This will print performance metrics to the console.
