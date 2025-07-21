# 🌾 SmartFarm: Crop Recommendation System

A Machine Learning-based web application that recommends the most suitable crop to cultivate based on soil and climate parameters like nitrogen, phosphorus, potassium, temperature, humidity, pH, and rainfall.

---

## 🚀 Project Overview

SmartFarm is designed to empower farmers and agricultural planners by providing intelligent crop recommendations tailored to specific environmental and soil conditions. It utilizes supervised machine learning models trained on historical agricultural data to predict the best crop for cultivation on a given land area. The application is deployed using a Flask backend with a simple and interactive web interface.

---

## 🔧 Tech Stack

- **Programming Language**: Python  
- **ML Libraries**: Scikit-learn, Pandas, NumPy  
- **Web Framework**: Flask (with Jinja2 templating)  
- **Model Deployment**: Pickle for model and scaler serialization  
- **Frontend**: HTML, CSS  

---

## 🧠 Features

- Trained and evaluated multiple ML models:
  - Logistic Regression
  - Naive Bayes
  - Support Vector Machine (SVM)
  - Decision Tree
  - Gradient Boosting
  - AdaBoost
- **Final Model Chosen**: Naive Bayes Classifier  
  - Achieved **99.54% accuracy** on test data  
- **Feature Scaling**:
  - Used both **MinMaxScaler** and **StandardScaler** for preprocessing
- **Web Interface**:
  - Built using **Flask** and rendered via **Jinja2** templates
- **Deployment Ready**:
  - ML model and scalers are serialized using **pickle**
- **User-Friendly UI**:
  - Simple form to input soil and weather parameters
  - Instant recommendation of the best crop to grow

---

## 📁 Project Structure

├── app.py # Flask app for backend and routing
├── CROP_RECOMMENDATION.ipynb # Jupyter Notebook with model training and evaluation
├── Crop_recommendation.csv # Dataset used for model training
├── model.pkl # Trained Naive Bayes model
├── minmaxscaler.pkl # Serialized MinMaxScaler
├── standscaler.pkl # Serialized StandardScaler
├── templates/
│ └── index.html # Frontend UI using Jinja2
├── static/
│ └── style.css # Optional CSS styling for UI
├── Logo.png # Optional logo for UI
└── README.md # Project documentation


---

## 💡 How It Works

1. User enters values for Nitrogen, Phosphorus, Potassium, Temperature, Humidity, pH, and Rainfall.
2. The input is preprocessed using saved scalers.
3. The trained Naive Bayes model predicts the best crop based on the input.
4. The result is displayed on the UI instantly.

---

## 📊 Dataset Source

- **Crop Recommendation Dataset**: [Kaggle - Crop Recommendation Dataset](https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset)

---

## 🚀 Future Enhancements

- Integrate satellite or real-time weather APIs for automatic parameter fetching
- Add multilingual support for farmers in different regions
- Mobile-responsive UI for easy access
- Extend to pest/disease prediction for complete smart farming



