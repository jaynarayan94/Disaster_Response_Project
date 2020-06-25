# Disaster Response Project
## Introduction  
The project is to create a web interface where you have to enter a disaster message and it will categorize the type of message.
This will help in effective response and action to be taken on each message. The data's used in this project is shared by Figure Eight in collaboration with Udacity.The dataset is a combination of pre-labelled tweet and messages from real-life disastero collected from different sources.
</br>

<span>
<img src="https://github.com/jaynarayan94/Disaster_Response_Project/blob/master/Images/Web%20Layout.png" width=220px height="300px" />
<img src="https://github.com/jaynarayan94/Disaster_Response_Project/blob/master/Images/Web%20Layout2.png" width=230px height="300px" />
</span>

### Dependencies Tools/Libraries
* Python 3+
* Scikit-Learn 0.22.1
* Numpy, Pandas
* NLTK, re
* Joblib
* SQLalchemy
* HTML & CSS
* Flask

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
        
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`
   Your web app should now be running if there were no errors.
   
3. Now, open another Terminal Window.
    Type : env|grep WORK
    
4. In a new web browser window, type in the following:
    https://SPACEID-3001.SPACEDOMAIN
    
 Your SPACEID & SPACEDOMAIN might be unique.
 You should be able to see the web app. The number 3001 represents the port where your web app will show up. Make sure that the 3001 is part of the web address you type in.

5. Go to http://0.0.0.0:3001/

### File structure of the project:
#### - app
##### -| - template
##### | |- master.html  # main page of web app
##### | |- go.html  # classification result page of web app
##### |- run.py  # Flask file that runs app

#### - data
##### |- disaster_categories.csv  # data to process 
##### |- disaster_messages.csv  # data to process
##### |- process_data.py
##### |- InsertDatabaseName.db   # database to save clean data to

#### - models
##### |- train_classifier.py
##### |- classifier.pkl  # saved model 

#### - README.md

<a name="license"></a>
## License [2020 Jay Narayan]
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Issue/Bug
Please open issues on github to report bugs or make feature requests or drop a mail to "jaynarayan94@gmail.com"

