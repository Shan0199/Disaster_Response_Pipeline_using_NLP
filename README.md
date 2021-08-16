# Disaster Response Pipeline Project

## Project Motivation

In this project,Data Engineering skills are applied to analyze disaster data from Figure Eight to build a Supervised Machine Learning Model for an API that classifies disaster messages into Categories of disaster.

## File Description

    .
    ├── app     
    │   ├── run.py                           # Flask file that runs app
    │   └── templates   
    │       ├── classify.html                # Classification result page of web app
    │       └── Main.html                    # Main page of web app    
    ├── data                   
    │   ├── disaster_categories.csv          # Dataset including all the categories  
    │   ├── disaster_messages.csv            # Dataset including all the messages
    │   └── process_data.py                  # Data cleaning
    ├── models
    │   └── train_classifier.py              # Train ML model           
    └── README.md

### Instructions: (Run run.py) 
#### [DisasterResponse.db and classifier.pkl already exist.]
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

![Image](Disaster-Response.png)

## Example
Type in: We have a Storm and Fire breakout at Children's Park, New Delhi.

![Image](Classification.png)
