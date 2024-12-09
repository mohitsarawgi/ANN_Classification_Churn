# ANN_classification_Churn


# Overview
This project demonstrates how to use an Artificial Neural Network (ANN) to classify customer churn based on various features such as customer demographics, account information, and usage statistics. The model is implemented using TensorFlow and Keras, and the project includes preprocessing, model training, and evaluation.

# Features
Preprocessing customer data using techniques like scaling and encoding.
Building and training an Artificial Neural Network for binary classification.
Evaluating model performance using metrics like accuracy and confusion matrix.
Interactive interface using Streamlit for predictions and insights.


# Installation

Clone the Repository

bash
Copy code
git clone https://github.com/mohitsarawgi/ANN-Classification-Churn.git
cd ann-classification-churn
Create a Virtual Environment
##
bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install Dependencies
##
bash
Copy code
pip install -r requirements.txt
Download Dataset

Place your dataset in the root folder of the project. Update the file name in the script if needed.
Usage
Run the Streamlit Application

bash
Copy code
streamlit run app.py
Access the Application

Open your browser and navigate to http://localhost:8501.
Make Predictions

Upload customer data through the Streamlit app or use sample data for predictions.
Project Structure
bash
Copy code
ann-classification-churn/
│
├── app.py                     # Streamlit application script
├── model.py                   # ANN model creation and training
├── preprocess.py              # Data preprocessing utilities
├── requirements.txt           # Project dependencies
├── README.md                  # Project documentation
├── dataset/                   # Folder for input data
│   └── customer_churn.csv     # Example dataset
└── models/                    # Folder for saved models
    └── ann_model.h5           # Trained ANN model


