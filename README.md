🩺 Disease Prediction from Symptoms

An AI/ML based disease prediction system that predicts possible diseases based on symptoms entered by the user.
The model is trained using a medical symptom dataset and deployed through an interactive Gradio interface.

This project demonstrates machine learning, data preprocessing, and interactive AI application deployment.

🚀 Project Overview

The system takes a list of user-selected symptoms and predicts the most likely disease using a trained Random Forest Classifier.

It converts symptoms into a machine-readable format and uses a trained ML model to make predictions.

This project showcases:

Machine Learning Model Development

Data Preprocessing

Feature Engineering

Model Training & Evaluation

Interactive AI Interface using Gradio

🛠️ Technologies Used

Python

Pandas – Data processing

Scikit-learn – Machine Learning

Random Forest Classifier

Gradio – Web interface for predictions

Google Colab / Jupyter Notebook

⚙️ How It Works
1️⃣ Dataset Loading

The dataset contains multiple symptoms as features and the disease as the target label.

2️⃣ Data Preprocessing

Removed unnecessary column (Unnamed:133)

Converted symptoms into numerical features

Separated features and target
X = df.iloc[:, :-1]
y = df['prognosis']

3️⃣ Train/Test Split

Dataset is divided into training and testing data to evaluate model performance.
train_test_split(X, y, test_size=0.2)

4️⃣ Model Training

A Random Forest Classifier is used because it performs well on classification tasks and handles feature interactions effectively.

model = RandomForestClassifier()
model.fit(X_train, y_train)

5️⃣ Disease Prediction

The model predicts the disease based on selected symptoms.
prediction = model.predict(input_symptoms)

6️⃣ Gradio Interface

An interactive UI allows users to select symptoms and get predictions instantly.
gr.Interface()

📊 Features

✔ Predict diseases based on symptoms
✔ Interactive web interface using Gradio
✔ Machine learning classification model
✔ Clean and simple implementation
✔ Easy to extend with more datasets

📈 Future Improvements

Add deep learning models

Use larger medical datasets

Improve prediction accuracy

Deploy as a full web application

Add top 3 disease predictions
