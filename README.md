

---

# Customer Churn Prediction  

This repository contains the code and resources for the **Customer Churn Prediction** project, which utilizes machine learning techniques to predict customer churn. By analyzing customer data, the project identifies patterns that help businesses understand customer retention and behavior.

## Table of Contents  
1. [Overview](#overview)  
2. [Dataset](#dataset)  
3. [Model](#model)  
4. [Installation](#installation)  
5. [Results](#results)  
6. [Contributing](#contributing)  
7. [Acknowledgements](#acknowledgements)  

## Overview  
The **Customer Churn Prediction** project aims to assist businesses in identifying customers likely to churn by leveraging machine learning models. This project analyzes customer data, preprocesses it for model training, and evaluates predictions to improve customer retention strategies.

## Dataset  
The dataset used for this project contains customer information, including demographic details, service subscriptions, and account status. It consists of 21 features, with the target variable being `Churn`, which indicates whether a customer has churned (1) or not (0).

### Features:
- **customerID**: Unique identifier for each customer  
- **gender**: Gender of the customer  
- **SeniorCitizen**: Whether the customer is a senior citizen (1 if yes, 0 if no)  
- **Partner**: Whether the customer has a partner (Yes/No)  
- **Dependents**: Whether the customer has dependents (Yes/No)  
- **tenure**: The number of months the customer has been with the company  
- **PhoneService**: Whether the customer subscribes to phone service (Yes/No)  
- **MultipleLines**: Whether the customer has multiple lines (Yes/No)  
- **InternetService**: Type of internet service (Fiber optic, DSL, No)  
- **OnlineSecurity**: Whether the customer subscribes to online security (Yes/No)  
- **DeviceProtection**: Whether the customer subscribes to device protection (Yes/No)  
- **TechSupport**: Whether the customer subscribes to tech support (Yes/No)  
- **StreamingTV**: Whether the customer subscribes to streaming TV (Yes/No)  
- **StreamingMovies**: Whether the customer subscribes to streaming movies (Yes/No)  
- **Contract**: Type of contract (Month-to-month, One year, Two year)  
- **PaperlessBilling**: Whether the customer uses paperless billing (Yes/No)  
- **PaymentMethod**: Payment method used (e.g., Bank transfer, Credit card)  
- **MonthlyCharges**: Monthly charges for services  
- **TotalCharges**: Total charges for the customer  
- **Churn**: Target variable indicating whether the customer has churned (Yes/No)

## Model  
The project utilizes a **deep learning-based Artificial Neural Network (ANN)** for predicting churn. The model pipeline includes:  
- **Data Preprocessing**: Handling missing values, encoding categorical variables, and scaling numerical features.  
- **Model Architecture**: Fully connected layers with activation functions to classify churn.  
- **Evaluation Metrics**: Accuracy, precision, recall, and F1-score.  

## Installation  
To run this project locally, follow these steps:

1. Clone the repository:  
   ```bash  
   git clone <repository_link>  
   ```  

2. Navigate to the project directory:  
   ```bash  
   cd Customer-Churn-Prediction  
   ```  

3. Create and activate a virtual environment:  
   ```bash  
   python -m venv venv  
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`  
   ```  

4. Install the required packages:  
   ```bash  
   pip install -r requirements.txt  
   ```  

## Results  
The ANN model's performance on the test dataset is summarized below:  

- **Accuracy:** 78%  
- **Precision (Class 0 - Did not churn):** 83%  
- **Precision (Class 1 - Churned):** 63%  
- **Recall (Class 0 - Did not churn):** 86%  
- **Recall (Class 1 - Churned):** 56%  

These metrics highlight the model's ability to predict customer churn effectively, with a strong performance for identifying customers who did not churn.

## Contributing  
Contributions are welcome! If you have any suggestions or improvements, feel free to open an issue or create a pull request.  

## Acknowledgements  
- Special thanks to https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling for providing the customer data.  
- Thanks to the TensorFlow and Keras teams for their robust frameworks.  


