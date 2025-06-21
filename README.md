Diabetes Prediction Project
Project Description
This project aims to predict the likelihood of diabetes in patients based on diagnostic measurements. The project utilizes the Pima Indians Diabetes Database to train a Support Vector Machine (SVM) model for classification.

Data Description
The dataset used in this project is the Pima Indians Diabetes Database. It contains health information about female patients of Pima Indian heritage. The dataset includes 768 instances and 9 attributes.

The attributes are:

Pregnancies: Number of times pregnant
Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
BloodPressure: Diastolic blood pressure (mm Hg)
SkinThickness: Triceps skin fold thickness (mm)
Insulin: 2-Hour serum insulin (mu U/ml)
BMI: Body mass index (weight in kg/(height in m)^2)
DiabetesPedigreeFunction: Diabetes pedigree function
Age: Age (years)
Outcome: Class variable (0 for no diabetes, 1 for diabetes)
Methodology
The project follows these steps:

Data Loading: The diabetes.csv file is loaded into a pandas DataFrame.
Data Exploration: Initial data exploration is performed using head(), shape, describe(), value_counts() on the 'Outcome' column, and groupby('Outcome').mean() to understand the data distribution and relationships.
Data Preprocessing:
Features (X) and labels (Y) are separated, with 'Outcome' as the label.
The feature data is standardized using StandardScaler to ensure all features have a similar range.
Model Training: A Support Vector Machine (SVM) classifier with a linear kernel is initialized and trained on the standardized training data.
Model Evaluation: The trained model's accuracy is evaluated on both the training and test sets using the accuracy_score metric.
Prediction: The trained model is used to make predictions on new input data after standardizing it.
Results
The trained SVM model achieved the following accuracy scores:

Training Accuracy: 0.7866
Test Accuracy: 0.7727
This indicates that the model performs reasonably well in predicting diabetes on both seen and unseen data.

How to Run the Code
To run this notebook, you need to have Python and the following libraries installed:

pandas
numpy
scikit-learn
You can install the dependencies using pip:
