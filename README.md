
# 🚦 ML Final Project: Traffic Congestion Level Prediction 🚗

Welcome to the Traffic Congestion Level Prediction project! This project predicts traffic congestion levels (Low, Medium, High) using machine learning techniques like Random Forest with One-vs-Rest strategy, along with data preprocessing, balancing using SMOTE, and detailed evaluation metrics.

---

## 📂 Project Structure

```
.
├── train.py              # Train the machine learning model
├── test.py               # Test and evaluate the model
├── data_cleaned.csv      # Cleaned dataset used for training and testing
├── model.joblib          # Trained model (generated after running train.py)
├── scaler.joblib         # Scaler for feature normalization (generated after running train.py)
├── label_encoder.joblib  # Encoder for target labels (generated after running train.py)    
└── README.md             # Project documentation (this file)
```

---

## ⚙️ Requirements

- Python 3.x

Install dependencies using pip:

To install the necessary libraries use:

```bash
pip install pandas numpy scikit-learn imbalanced-learn joblib
```

---

## 📄 Files Description

### `train.py`
✅ Loads and preprocesses the data.  
✅ Encodes categorical features and target variable.  
✅ Applies SMOTE to balance the dataset.  
✅ Scales features using StandardScaler.  
✅ Trains a Random Forest classifier with One-vs-Rest strategy.  
✅ Saves the trained model, scaler, and label encoder for future use.

### `test.py`
✅ Loads the saved model, scaler, and label encoder.  
✅ Prepares the test dataset.  
✅ Performs predictions on the test data.  
✅ Outputs evaluation metrics like accuracy, precision, recall, F1 score, classification report, and confusion matrix.

---

## 🚀 How to Run

### Step 1: Train the model

```bash
python train.py
```

After successful execution, you will get:

- `model.joblib`
- `scaler.joblib`
- `label_encoder.joblib`

### Step 2: Test the model

```bash
python test.py
```

You will see performance metrics printed in your console.



---


