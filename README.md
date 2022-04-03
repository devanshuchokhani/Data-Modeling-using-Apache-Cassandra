# Udacity Data Engineer Nanodegree Project: Data Modeling with Apache Cassandra

## Introduction
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

They'd like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions, and wish to bring you on the project. Your role is to create a database for this analysis. You'll be able to test your database by running queries given to you by the analytics team from Sparkify to create the results.

## Project pipeline and data modelling

The project template includes one Jupyter Notebook file, in which:
* creating event_datafile_new.csv dataset
* creating denormalized tables according to the requirements
* loading the data into tables
* running queries to validate results

Pipeline generates the following tables:
* artist_song_length: artist, song title and song length information for a given sessionId and itemInSessionId
* artist_song_user: artist, song and user for a given userId and sessionId
* user: user names for a given song
