
*"The course that we're doing is the [Intro to SQL](https://www.kaggle.com/learn/intro-to-sql) course, with some additional stuff from me" -- Rachael Tatman (Livestream, Day1 1'08)*

*"BigQuery [from Google] is just where the data[set] that we want to query is [hosted] ... The SQL syntax is going to be the same, more or less ... no matter what service you use" -- Rachael Tatman (Livestream, Day1 9'16)*

*"One really nice thing is that you don't actually have to setup any authentication, to use BigQuery data on Kaggle" -- Rachael Tatman (Livestream, Day1 9'53)*


## Day 1 (2019-06-25)

"Today we’re going to learn what relational databases [are], when you should use them and how to interact with SQL datasets on Kaggle. Let’s jump right in"

* **1. Getting Started with SQL and BigQuery** : [Notebook](https://www.kaggle.com/dansbecker/getting-started-with-sql-and-bigquery) with lesson
* **2. Exercise : Getting Started with SQL and BigQuery** : [Notebook](https://www.kaggle.com/mbeveridge/exercise-getting-started-with-sql-and-bigquery/edit) with exercises. (If you want to save your work, be sure to sign in to your Kaggle account! ...*else work will disappear after 15min*)
* [Livestream (recording 25/6/19)](https://www.youtube.com/watch?v=jYQoQfFzJRw) (~30min + 30min Q&A) [*@31'45 how to use R instead of Python*] [*@38'50-39'40 What problem does BigQuery solve? Run queries v quickly, even if dataset is v large*] [*@46'45-48'30 Link to all the BigQuery client commands*] [*48'40-49'00 Can we use BigQuery with R?*] [*@57'10-57'55 What can you not do with pandas that you can do with SQL (after you've imported a dataset to a dataframe)? Not much. With SQL, you don't have to have your data locally (re. size). And SQL tends to be a bit quicker, for same size of data*]

*To use BigQuery, we'll import the Python package `bigquery`. Then create a `Client` object. Create a reference to our `hacker_news` dataset (which is in `bigquery-public-data` project) and then we can fetch the dataset. Similarly, create a reference to an individual table (which is in the dataset) and then we can fetch the table*

*'Kaggle > Discussion > Learn' for the forum, to ask questions*


## Day 2

"Now that you know what relational databases are and how to access BigQuery data on Kaggle we’re ready to start writing SQL code. Today we’ll cover the basic building blocks of SQL queries: select, from and where"

* Notebook with today’s lesson
* Exercise for the lesson
* Livestream (recording) from 4:00 PM GMT


## Day 3

"Today we’re going to learn how to write SQL queries that will help summarize the data in the database and let you ask more complicated questions"

* Notebook with today’s lesson
* Exercise for the lesson
* Livestream (recording) from 4:00 PM GMT
