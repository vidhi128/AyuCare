🌿 AyuCare – Disease Prediction & Medicine Recommendation System

A Machine Learning + Flask Web Application for Smart Healthcare Assistance

📌 Project Overview

AyuCare is a healthcare web application that assists users by:

Predicting diseases based on selected symptoms

Recommending suitable medicines based on predicted disease, gender, age & severity

Providing a secure user authentication system

Offering a clean UI to interact with ML models

This project leverages Machine Learning, Flask, SQLite, and WTForms to deliver accurate predictions and a seamless user experience.

🚀 Features
🔹 1. Disease Prediction

Uses a trained Decision Tree Classifier

Takes multiple symptoms as input

Converts symptoms → one-hot encoded vector → model prediction

Returns disease name with high accuracy

🔹 2. Medicine Recommendation

Uses a second ML model (drugTree.pkl)

Inputs:

Disease

Gender

Age

Severity level

Recommends the best medicine based on model predictions

🔹 3. User Authentication

Register / Login pages

Password hashing using Flask-Bcrypt

User session handling using Flask-Login

🔹 4. Database Support

SQLite database to store:

Users

Health details

Past conditions

🔹 5. User-Friendly UI

HTML templates with clean layout

Dropdown-based selections for symptoms, diseases, severity, gender

🧠 Machine Learning Models

Two ML models are used:

1. Disease Detection Model

Algorithm: Decision Tree

Input: 30 symptoms (one-hot encoded)

Output: Disease category

File: DecisionTree-Model.sav

2. Medicine Recommendation Model

Algorithm: Decision Tree

Input: [disease, age, gender, severity]

Output: Recommended medicine

File: drugTree.pkl

🗂️ Project Structure
AyuCare/
│── app.py
│── database.db (auto-created)
│── DecisionTree-Model.sav
│── drugTree.pkl
│── static/
│   └── assets/
│── templates/
│   ├── index.html
│   ├── signin.html
│   ├── register.html
│   ├── service.html
│   ├── med_service.html
│   ├── doc_service.html
│── <team-member-folders>/
│── README.md
│── .gitignore

🛠️ Tech Stack
Backend

Python

Flask

SQLAlchemy

Flask-Login

Flask-WTF

Flask-Bcrypt

Machine Learning

Scikit-Learn

NumPy

Pandas

Joblib / Pickle

Frontend

HTML

CSS

Bootstrap / Tailwind classes

Database

SQLite

▶️ How to Run the Project Locally
1. Clone the Repository
git clone https://github.com/vidhi128/AyuCare.git
cd AyuCare

2. Create Virtual Environment
python -m venv venv

3. Activate Environment

Windows:

venv\Scripts\activate

4. Install Required Libraries
pip install -r requirements.txt

5. Run the Flask App
python app.py


Visit:
👉 http://127.0.0.1:5000/



My Role in This Project:

✔ Implemented the Disease Prediction Model using Decision Tree
✔ Created feature-engineering pipeline for symptoms
✔ Trained the Medicine Recommendation Model
✔ Handled model integration inside Flask routes
✔ Debugged compatibility issues and ensured correct Python-scikit-learn versions
✔ Helped in folder restructuring + GitHub deployment
