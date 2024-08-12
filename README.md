## Student Performance Prediction - End to End Machine Learning Project Deployed on AWS EC2

This repository contains an end-to-end machine learning project focused on predicting the performance of high school students in mathematics based on their demographic information and other relevant factors.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training](#model-training)
- [Prediction Pipeline](#prediction-pipeline)
- [Deployment](#deployment)
- [Video Demo](#video-demo)

## Project Overview
The goal of this project is to develop a machine learning model that can predict a student's math score based on various features such as gender, race/ethnicity, parental level of education, lunch type, test preparation course, reading score, and writing score. The project includes data ingestion, data transformation, model training, and deployment on AWS EC2.

## Dataset
### Description
This dataset contains information on the performance of high school students in mathematics, including their grades and demographic information. The data was collected from three high schools in the United States.
Dataset Link: https://www.kaggle.com/datasets/rkiattisak/student-performance-in-mathematics

### Columns
- **Gender**: The gender of the student (male/female)
- **Race/Ethnicity**: The student's racial or ethnic background (Asian, African-American, Hispanic, etc.)
- **Parental Level of Education**: The highest level of education attained by the student's parent(s) or guardian(s)
- **Lunch**: Whether the student receives free or reduced-price lunch (yes/no)
- **Test Preparation Course**: Whether the student completed a test preparation course (yes/no)
- **Math Score**: The student's score on a standardized mathematics test
- **Reading Score**: The student's score on a standardized reading test
- **Writing Score**: The student's score on a standardized writing test


## Installation
To get started with the project, clone the repository and install the necessary dependencies:

```bash
git clone https://https://github.com/areebbinnadeem/ML-Projects
cd ML-Projects
pip install -r requirements.txt
```


## Usage

### Running the Application
Start the Flask application:

```bash
python application.py
```


Open your browser and go to http://localhost:8080/ to access the home page.

Input the required details in the form and get the predicted math score for a student.

## Files and Folders
- **artifacts/** : Contains the preprocessed data, trained models, and other artifacts.
- **notebook/** : Contains Jupyter notebooks for exploratory data analysis (EDA) and model training.
- **src/** : Contains the source code for data ingestion, data transformation, model training, and prediction pipelines.
- **static/ and templates/** : Contain static files and HTML templates for the web application.
- **application.py** : The main Flask application file.
- **requirements.txt** : Lists the dependencies needed to run the project.
- **setup.py** : Setup script for packaging the project.

## Model Training

The model training process involves the following steps:
1. **Data Ingestion:** The raw data is loaded, and train-test splits are created.
2. **Data Transformation:** Data is preprocessed using pipelines for numerical and categorical features.
3. **Model Training:** Multiple regression models are trained and evaluated using cross-validation.
4. **Model Selection:** The best-performing model is selected based on R² score and saved as a pickle file.

## Prediction Pipeline

The prediction pipeline involves:
The model training process involves the following steps:
1. Loading the trained model and preprocessor.
2. Transforming the input data using the preprocessor.
3. Predicting the math score using the trained model.
4. Returning the predicted score to the user.

## Deployment
The application was deployed on AWS EC2 using PUTTY and WINSCP by following the below steps:
1. Set up an AWS EC2 instance and connect to it using SSH.
2. Transferred the project files to the instance using SCP.
3. Installed the required dependencies on the instance.
4. Ran the Flask application on the server and accessed it via the public IP address provided by the EC2 instance.

## Video Demo

[![Watch the video]](https://youtu.be/TOCwU-qzhb4)