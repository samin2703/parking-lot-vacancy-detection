This project implements a machine learning model to detect parking lot vacancies using image data. The system classifies images into two categories: empty and not_empty, enabling efficient monitoring of parking spaces.


![Parking Lot Detection Demo](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExYzA2OXBmeXloeG13Z2NnNGg4dXhjcWN3dTBmYjZ5NWV4MnNua3FkZiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/EFGDfCzS5YA48/giphy.gif)

**Features**

Image Preprocessing: Resizes and flattens images for consistent input to the model.

Model Training: Utilizes a Support Vector Machine (SVM) classifier with hyperparameter tuning through RandomizedSearchCV for efficient optimization.

Real-Time Predictions: Capable of predicting parking lot occupancy based on input images.

Model Persistence: Trained model is saved as a .p file for future use.

Customizability: Easy to expand for additional categories or real-time video analysis.

**Technologies Used**

Python: For overall implementation.

NumPy: For numerical computations.

scikit-image: For image loading and preprocessing.

scikit-learn: For machine learning model training and evaluation.

**How It Works**

Dataset Preparation:

Images are categorized as empty or not_empty.
Each image is resized to 15x15 pixels and flattened for model input.

**Model Training:**

SVM classifier is trained with a dataset of parking lot images.
RandomizedSearchCV is used to fine-tune the gamma and C parameters for the SVM.

**Prediction:**

Trained model predicts the category of a new parking lot image.
Output specifies whether the parking lot is vacant or occupied.
Usage

Train the model using provided image data.

Use the saved model to predict parking lot vacancies for new images.
Integrate the prediction functionality with a live camera feed for real-time monitoring.
