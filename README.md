# Disaster Response Pipeline Project (Udacity - Data Science Nanodegree Project)


## Table of Contents
1. [Description](#description)
2. [Dependencies](#dependencies)
3. [Installing](#installation)
4. [Executing Program](#execution)
5. [Authors](#authors)
6. [License](#license)
7. [Acknowledgement](#acknowledgement)

<a name="description"></a>
## Description

This project is a join collaboration between Udacity and Figure Eight. This project revolves around messages received from real-life disaster events. The purpose of this project is to categorize these messages in real-time by building a Natural Language Processing model.

__This project goes as follows:__
1. Processing data, building an ETL pipeline to extract data from source, clean the data and save them in a SQLite DB
2. Build a machine learning pipeline to train the which can classify text message in various categories
3. Run a web app which can show model results in real time

<a name="dependencies"></a>
### Dependencies
* Python 3.5+
* Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
* Natural Language Process Libraries: NLTK
* SQLlite Database Libraqries: SQLalchemy
* Model Loading and Saving Library: Pickle
* Web App and Data Visualization: Flask, Plotly

<a name="installation"></a>
### Installing
To clone the git repository:
```
git clone https://github.com/HunterKane/Disaster-Response-Project.git 

```
<a name="execution"></a>
### Executing Program:
1. You can run the following commands in the project's directory to set up the database, train model and save the model.

    - To run ETL pipeline to clean data and store the processed data in the database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/disaster_response_db.db`
    - To run the ML pipeline that loads data from DB, trains classifier and saves the classifier as a pickle file
        `python models/train_classifier.py data/disaster_response_db.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

<a name="authors"></a>
## Authors

* [Hunter Sparrow](https://github.com/HunterKane)

<a name="license"></a>
## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<a name="acknowledgement"></a>
## Acknowledgements

This project could not have been completed without the collaboration of these two contributors:

* [Udacity](https://www.udacity.com/) for providing the learning platform. 
* [Figure Eight](https://www.figure-eight.com/) for providing the relevant dataset
