# Disease Prediction System

---

## Overview

---

This is a Flask-based web application that uses machine learning to predict diseases based on user-inputted symptoms. The system uses a Support Vector Machine (SVM) model to classify diseases and provides recommendations for precautions, medication, diet, and workout.

## Features

---

* Predicts diseases based on user-inputted symptoms
* Provides recommendations for precautions, medication, diet, and workout
* Uses a Support Vector Machine (SVM) model for classification
* Loads datasets from CSV files
* Saves and loads the trained model using pickle

## How to Use

---

1. Run the application by executing `python main.py`
2. Open a web browser and navigate to `http://localhost:5000`
3. Input your symptoms in the text box, separated by commas
4. Click the "Predict" button to get the predicted disease and recommendations

## Run with Docker

---

1. Build the Docker image:

   ```bash
   docker build -t disease-detection-app .
   ```
2. Run the container:

   ```bash
   docker run --rm -p 5000:5000 disease-detection-app
   ```
3. Open your browser at `http://localhost:5000`

## Technical Details

---

* The application uses Flask as the web framework
* The SVM model is trained using scikit-learn
* The datasets are loaded from CSV files using pandas
* The application uses pickle to save and load the trained model

## Files

---

* `app.py`: the main application file
* `Dataset/Training.csv`: the training dataset
* `Dataset/precautions_df.csv`: the precautions dataset
* `Dataset/workout_df.csv`: the workout dataset
* `Dataset/description.csv`: the description dataset
* `Dataset/medications.csv`: the medication dataset
* `Dataset/diets.csv`: the diet dataset
* `model/svc.pkl`: the saved SVM model
* `templates/index.html`: the HTML template for the user interface

## License

---

This application is licensed under the MIT License. See `LICENSE` for details.
