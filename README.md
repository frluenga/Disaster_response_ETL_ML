# Disaster Response Pipeline Project

## Project Description
In this project, a machine learning model is developed with an automated pipeline that receives a dataset with messages of possible emergencies or categorized disasters respectively. The goal of the project is to build a basic ETL and machine learning pipeline to make the task easier. It is a multi-tag classification because a message can belong to one or more categories. We will be working with a data set provided by [Figure Eight](https://www.figure-eight.com/) that contains actual messages that were sent during disasters.

Preparation folder is not necessary for this project to run.

## File Description
~~~~~~~
        disaster_response_pipeline
          |-- app
                |-- templates
                        |-- go.html
                        |-- master.html
                |-- run.py
          |-- data
                |-- disaster_message.csv
                |-- disaster_categories.csv
                |-- DisasterResponse.db
                |-- process_data.py
          |-- models
                |-- classifier.pkl
                |-- train_classifier.py
          |-- README
~~~~~~~
## Installation
It should be run with Python with the following libraries:
 - numpy 
 - pandas 
 - sqlalchemy
 - re
 - NLTK
 - pickle
 - Sklearn
 - plotly 
 - flask libraries.

## File Descriptions
1. App folder including the templates folder and "run.py" for the web application
2. Data folder containing "DisasterResponse.db", "disaster_categories.csv", "disaster_messages.csv" and "process_data.py".
3. Models folder including "classifier.pkl" and "train_classifier.py" for the Machine Learning model.
4. README file


## Instructions
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3000/

## Licensing, Authors, Acknowledgements
Many thanks to Figure-8 for making this available to Udacity for training purposes. Special thanks to udacity for the training. Feel free to utilize the contents of this while citing me, udacity, and/or figure-8 accordingly.
