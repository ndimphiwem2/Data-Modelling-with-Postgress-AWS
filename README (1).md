The Purpose of the Database:

The aim of the database is to specially organise the data collected for a startup music streaming organisation called Sparkify. The database is created to optimise querries on song play analysis. A database Schema was created to be able to store the data and retrieve it for analysis. The data was originally saved as a JSON file which is not easy to query for aggregation purposes.

Python Scripts can be run as follows:

The python scripts(.py files) can be run by going to file, then new, then terminal. Once on terminal, a user can write a command to run the python script. For example, if you want to run etl.py script, you can type "python etl.py", then press enter to run the script. 


Files in the Repository

There are seven (files in the respository), each with a specific purpose but they all work together as one project.
File 1 - Data - this is where the raw data stored as a JSON file.Song_data and log_data are both stored here.
File 2 - Create_tables.py - contains python/SQL commands that drops and creates tables in the database.
File 3 - etl.ipynb - this is a jupiter notebook file that reads and processes a single file from the song data and log data and load the data into tables in the database.
File 4 - etl.py - this is a python script that reads and processes files from the song_data and log_data and loads them into tables in the database.
File 5 - README.md provides detailes about what the project is all about and how to execute it.
File 6 - sql_queries.py - this is a python script that contains all the sql querries.
File 7 - test.ipynb - this is a jupiter notebook that is used to test if the data is indeed loaded into the tables in the database. It displays the first few rows of each table.


Database Schema design and ETL pipelines:

A star database schema design was chosen as the best schema to be used for heavy retrieval of data and for aggregation analytics purposes.

My star schema has one fact table - songplays and  four dimension tables which are users, songs, artists, time. 

Extract Transform and Load (ETL) Pipilines

ETL pipelines were build on etl.py python scripts to process the entire dataset.




