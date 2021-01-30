# Sparkify Cassandra Database

## Project Description

The project is to create ***Apache Cassandra NoSQL database*** for Sparkify.  


The aim is to have a database which can provide answers for **3 types of questions**:  


1. Give me the **artist, song title and song's length** in the music app history that was heard as a **given item in a given session**.  
I.e. *SELECT artist, song, length FROM music_per_session WHERE sessionId = [] and itemInSession = [];*


2. Give me only the following: **name of artist, song (sorted by itemInSession) and user (first and last name)** for a **given userid and sessionid**.  
I.e. *SELECT artist, song, firstName, lastName FROM music_per_user_and_session WHERE userId = [] AND sessionId = [];*  


3. Give me every **user name (first and last)** in my music app history who listened the **specific song**.
I.e. *SELECT firstName, lastName FROM listeners_per_song WHERE song = [];*  


## Structure of the workspace

The workspace contains 4 objects:
- ***event_data*** folder stores csv files with events
- ***images*** folder stores an image of the data structure of the csv files
- ***Sparkify Cassandra ETL.ipynb*** is a Jupyter Notebook with the whole code for the project
- ***event_datafile_new.csv*** is a CSV file created during the project from files stored in the event_data folder. This is the data source for db tables.


## How to run the project

To run the project just go to the **Sparkify Cassandra ETL** notebook and run the code.  


You will find more comments in the notebook.