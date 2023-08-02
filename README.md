# Multiple Disease Detection App

This repository contains a Python script and a web-based GUI application built using Streamlit to predict three different medical conditions: diabetes, ❤️ heart disease, and 👤 Parkinson's disease. The application showcases the process of building predictive models for medical diagnosis.

## Multiple Disease Detection Script

### Purpose
The script demonstrates the development of a predictive model using the Support Vector Machine (SVM) algorithm to detect Parkinson's disease based on health metrics.

### Steps Covered
1. **Importing Dependencies**: Essential libraries such as numpy, pandas, and scikit-learn are imported for data manipulation, machine learning operations, and evaluation.

2. **Data Collection & Analysis**: Data is read from a CSV file using Pandas. The script displays initial data exploration results like the first few rows, data shape, column information, missing values check, and statistical summary.

3. **Data Pre-Processing**: The data is separated into features (X) and target labels (Y) by dropping the 'name' and 'status' columns.

4. **Splitting the Data**: The dataset is split into training and test sets using the train_test_split() function from scikit-learn. A random seed is set for reproducibility.

5. **Model Training (SVM)**: An SVM model with a linear kernel is instantiated and trained on the training data using the fit() method.

6. **Model Evaluation**: The accuracy of the trained SVM model is evaluated on both the training and test datasets using the accuracy_score() function.

7. **Building a Predictive System**: An example input data is provided, converted to a NumPy array, and reshaped to fit the model's input format. The trained model predicts whether the individual has Parkinson's disease based on the input data.

8. **Saving the Trained Model**: The script saves the trained SVM model using the pickle library. The saved model can be loaded and used for predictions without retraining.

9. **Loading and Using the Saved Model**: The script demonstrates loading the saved model and printing the feature column names.

In summary, this script showcases the complete workflow of loading, analyzing, preprocessing, training, evaluating, predicting, and saving an SVM model for detecting Parkinson's disease based on given health metrics.

## Web GUI Application

### Purpose
The web GUI application built using Streamlit allows users to interactively predict three medical conditions: diabetes, ❤️ heart disease, and 👤 Parkinson's disease.

### Steps Covered
1. **Importing Dependencies**: The application uses Streamlit for creating the web interface, the pickle library to load pre-trained models, and a custom module for navigation.

2. **Loading Saved Models**: Pre-trained models for each disease are loaded from corresponding files.

3. **Sidebar Navigation**: Users can navigate between different disease prediction options using the sidebar menu.

4. **Prediction Pages**: For each disease, a dedicated page collects user-input health metrics and displays the prediction result based on the corresponding pre-trained model.

5. **Overall Structure**: The application provides a user-friendly interface where users input their health metrics, the pre-trained models make predictions, and the results are immediately displayed.

## How to Use

1. Clone the repository.
2. Run the Multiple disease detection script using Python.
3. Run the Streamlit application script using the command `streamlit run multiple disease pred.py` in your local or app.py in your deployment environment.
4. Access the application via the provided local URL or the public URL.

This repository serves as both a practical example of machine learning application in medical diagnosis and a user-friendly interface for predicting various medical conditions based on user-provided health metrics.

## OUTPUT
![Image](https://github.com/VedantMandre/Multiple-Disease-Prediction-/assets/114442140/7bebe09f-758e-4600-a672-2c52726c64db)
