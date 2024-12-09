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
--------------------------------
bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install Dependencies
--------------------------------/n
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


# Technologies Used
Python: Programming language.
TensorFlow/Keras: Building and training the ANN model.
Scikit-learn: Preprocessing and evaluation.
Streamlit: Interactive user interface.
Pandas & NumPy: Data manipulation and analysis.
How it Works
Data Preprocessing

Missing values are handled, features are scaled using StandardScaler, and categorical variables are encoded using LabelEncoder or OneHotEncoder.
Model Architecture

Input Layer: Accepts preprocessed data features.
Hidden Layers: Two layers with ReLU activation for feature extraction.
Output Layer: Single neuron with sigmoid activation for binary classification.
Training

The model is compiled using the binary_crossentropy loss function and optimized with adam.
Performance is monitored using accuracy.
Evaluation

Evaluate model performance on test data using accuracy and confusion matrix.
Deployment

The trained model is integrated with a Streamlit application for real-time predictions.
Dataset
The dataset contains the following columns:

RowNumber: Index of the customer.
CustomerId: Unique ID for the customer.
Surname: Customer surname (excluded in modeling).
Geography: Location of the customer (OneHotEncoded).
Gender: Gender of the customer (LabelEncoded).
Age: Age of the customer.
Balance: Account balance of the customer.
Tenure: Number of years as a customer.
Exited: Binary target variable indicating churn.
Results
Achieved an accuracy of 85% on the test set.
Confusion Matrix and classification report are available in the Streamlit app.
Future Improvements
Add more features for better accuracy.
Use hyperparameter tuning techniques like GridSearchCV.
Test alternative architectures (e.g., LSTM, CNN) for better performance.
