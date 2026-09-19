# Brain Age Status Prediction Using Machine Learning

A web application that classifies a person's brain-age status ("Short Age" or "Long Age") from health and lifestyle data, and compares four machine learning classifiers on a 5,110-record healthcare dataset. No MRI or imaging is needed; the goal is a low-cost, accessible screening-style tool.

Built by a team of three as a B.Tech final-year project at CMR Technical Campus (2024-25).

## Overview

Brain-age estimation usually relies on expensive neuroimaging. This project takes a lighter approach: users register, log in, enter health details (age, BMI, glucose level, hypertension, heart disease, smoking status and so on), and the app returns a brain-age status prediction. A service-provider (admin) side lets you train and test models, view accuracy charts, and review predictions.

## Features

- User registration and login
- Form-based input of health attributes with instant prediction
- Admin (service provider) module to train and test models, view accuracy as bar, line, and pie charts, view prediction ratios, and download predicted data as Excel
- Users and predictions stored in MySQL through the Django ORM

## Dataset

- Structured healthcare data in CSV format: 5,110 records, 12 variables
- Features: gender, age, hypertension, heart disease, ever married, work type, residence type, average glucose level, BMI, smoking status
- Label: neurological disease (Yes/No)
- BMI has 201 missing values

## Models Compared

- Linear Support Vector Machine (SVM)
- Logistic Regression
- Decision Tree Classifier
- k-Nearest Neighbors (KNN)

Data is split 80/20 for training and testing, and the admin module reports each model's accuracy.

## Tech Stack

- Python, Pandas, NumPy, Scikit-learn, Matplotlib
- Flask (web interface) and Django ORM (backend)
- MySQL
- HTML, CSS, JavaScript

## Project Status and Future Work

- Retrain and evaluate the models on the full set of health features, and report precision, recall, and confusion matrices in addition to accuracy
- Handle class imbalance and missing BMI values more carefully
- Explore neuroimaging or cognitive-test features for true brain-age estimation
- Add real-time monitoring, health-record integration, and deep learning models

## Authors

Busani Chaitanya, V Sree Malya, Namala Dinesh Kumar
B.Tech CSE (Design), CMR Technical Campus
Contact: busani.chay@gmail.com

## License

MIT. See `LICENSE`.
