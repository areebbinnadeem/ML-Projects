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
- [Results](#results)
- [Deployment](#deployment)
- [Acknowledgments](#acknowledgments)

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


