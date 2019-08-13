# SQL Summer Camp 2019


*"The course that we're doing is the [Intro to SQL](https://www.kaggle.com/learn/intro-to-sql) course, with some additional stuff from me" -- Rachael Tatman (Livestream, Day1 [@1'03](https://youtu.be/jYQoQfFzJRw?t=63))*

*"BigQuery [from Google] is just where the data[set] that we want to query is [hosted] ... The SQL syntax is going to be the same, more or less ... no matter what service you use" -- Rachael Tatman (Livestream, Day1 [@9'00](https://youtu.be/jYQoQfFzJRw?t=540))*

*"One really nice thing is that you don't actually have to setup any authentication, to use BigQuery data on Kaggle" -- Rachael Tatman (Livestream, Day1 [@9'48](https://youtu.be/jYQoQfFzJRw?t=588))*


## Day 1 (2019-06-25)

"Today we’re going to learn what relational databases [are], when you should use them and how to interact with SQL datasets on Kaggle. Let’s jump right in"

* **1. Getting Started with SQL and BigQuery** : [Notebook](https://www.kaggle.com/dansbecker/getting-started-with-sql-and-bigquery) with lesson
* **2. Getting Started with SQL and BigQuery** : [Notebook](https://www.kaggle.com/mbeveridge/exercise-getting-started-with-sql-and-bigquery/edit) with exercises. (If you want to save your work, be sure to sign in to your Kaggle account! ...*else work will disappear after 15min*)
* [Livestream (recording 25/6/19)](https://www.youtube.com/watch?v=jYQoQfFzJRw) (~30min + 30min Q&A) [*[@31'40](https://youtu.be/jYQoQfFzJRw?t=1900) how to use R instead of Python*] [*[@38'50](https://youtu.be/jYQoQfFzJRw?t=2330)-39'40 What problem does BigQuery solve? Run queries v quickly, even if dataset is v large*] [*[@46'45](https://youtu.be/jYQoQfFzJRw?t=2805)-48'30 Link to all the [BigQuery client commands](https://googleapis.github.io/google-cloud-python/latest/bigquery/reference.html)*] [*[@48'40](https://youtu.be/jYQoQfFzJRw?t=2920)-49'00 Can we use BigQuery with R?*] [*[@57'10](https://youtu.be/jYQoQfFzJRw?t=3430)-57'55 What can you not do with pandas that you can do with SQL (after you've imported a dataset to a dataframe)? Not much. With SQL, you don't have to have your data locally (re. size). And SQL tends to be a bit quicker, for same size of data*]

*To use BigQuery, we'll import the Python package `bigquery`. Then create a `Client` object. Create a reference to our `hacker_news` dataset (which is in `bigquery-public-data` project) and then we can fetch the dataset. Similarly, create a reference to an individual table (which is in the dataset) and then we can fetch the table*

*Rachel's ['BigQuery Scratchpad'](https://www.kaggle.com/rebeccaturner/bigquery-scratchpad) kernel, created during Livestream*

*['Kaggle > Discussion > Learn'](https://www.kaggle.com/learn-forum) for the forum, to ask questions. Including "[Slides from the first SQL livestream](https://www.kaggle.com/learn-forum/97118)"*


## Day 2 (2019-06-26)

"Now that you know what relational databases are and how to access BigQuery data on Kaggle we’re ready to start writing SQL code. Today we’ll cover the basic building blocks of SQL queries: select, from and where"

* **3. Select, From & Where** : [Notebook](https://www.kaggle.com/dansbecker/select-from-where) with lesson
* **4. Select, From & Where** : [Notebook](https://www.kaggle.com/mbeveridge/exercise-select-from-where/edit) with exercises
* [Livestream (recording 26/6/19)](https://www.youtube.com/watch?v=VljQui5es7g) (~30min + 30min Q&A) [*[@15'50](https://youtu.be/VljQui5es7g?t=950) "Now let's write a query"*] [*[@21'45](https://youtu.be/VljQui5es7g?t=1305) "...more queries"*] [*[@29'39](https://youtu.be/VljQui5es7g?t=1779) "I only want to run jobs if they are less than 100MB"*] [*[@30'42](https://youtu.be/VljQui5es7g?t=1842) "No, it still worked [didn't give an error msg]. Oh, it's cos it's cached [which doesn't count against your quota]. Oh, I need to write a new query"*] [*[@33'05](https://youtu.be/VljQui5es7g?t=1985) "Let's answer some questions"*] [*[@35'50](https://youtu.be/VljQui5es7g?t=2150) "Filter based on '#bigquery' and you can see all of our BigQuery datasets"*] [*[@46'45](https://youtu.be/VljQui5es7g?t=2805) "The SQL itself is not case-sensitive, but the strings you pass to be evaluated are case-sentive"*] [*[@56'56](https://youtu.be/VljQui5es7g?t=3416) "Let's quickly write a little regular expression, cos I'm interested in this"*]

*['openaq' dataset](https://www.kaggle.com/open-aq/openaq) ...re. [@9'56](https://youtu.be/VljQui5es7g?t=596) Livestream*

*Rachel's ['Select, From, Where scratchpad'](https://www.kaggle.com/rebeccaturner/select-from-where-scratchpad) kernel, created during Livestream*

*['Kaggle > Discussion > Learn'](https://www.kaggle.com/learn-forum) for the forum, to ask questions*


## Day 3 (2019-06-27)

"Today we’re going to learn how to write SQL queries that will help summarize the data in the database and let you ask more complicated questions"

* **5. Group By, Having & Count** : [Notebook](https://www.kaggle.com/dansbecker/group-by-having-count) with lesson
* **6. Group By, Having & Count** : [Notebook](https://www.kaggle.com/mbeveridge/exercise-group-by-having-count/edit) with exercises
* [Livestream (recording 27/6/19)](https://www.youtube.com/watch?v=dV74IWUkI8Q) (~30min + 30min Q&A) [*[@4'11](https://youtu.be/dV74IWUkI8Q?t=251) "I can see that I have this kernel running. And you can only have 4 kernels running"*] [*[@6'06](https://youtu.be/dV74IWUkI8Q?t=366) "Today we're going to learn how to aggregate, and how to start asking questions using SQL code" (instead of Python, R)*] [*[@13'05](https://youtu.be/dV74IWUkI8Q?t=785) "'Having' lets you ... filter things once they've been grouped. It's very similar to Where, but Having works with Group By"*] [*[@28'20](https://youtu.be/dV74IWUkI8Q?t=1700) "Let's look at questions"*] [*[@30'42](https://youtu.be/dV74IWUkI8Q?t=1842) "Why is `bq_helper` sometimes referred to?" It's a library that Rachael created, but is no longer used [v's `client`], but some kernels still talk about it*] [*[@36'50](https://youtu.be/dV74IWUkI8Q?t=2210) `COUNT(*)` v's `COUNT(1)` v's `COUNT(id)`*]

*Rachel's ['Group by, having & count scratchpad'](https://www.kaggle.com/rebeccaturner/group-by-having-count-scratchpad) kernel, created during Livestream*

*['Kaggle > Discussion > Learn'](https://www.kaggle.com/learn-forum) for the forum, to ask questions*


## Day 4 (2019-07-16)

"Today we’re going to talk about how to sort the data you get back from your query and, even more importantly, how to deal with dates"

* **7. Order By, Extract & Dates** : [Notebook](https://www.kaggle.com/dansbecker/order-by) with lesson
* **8. Order By, Extract & Dates** : [Notebook](https://www.kaggle.com/mbeveridge/kernelafe7322583/edit) with exercises
* [Livestream (recording 16/7/19)](https://www.youtube.com/watch?v=jEdgQ-RVmXw) (~30min + 30min Q&A) [*[@4'00](https://youtu.be/jEdgQ-RVmXw?t=240) "That's not so good. So I should be able to see a copy of the data in the database"*] [*[@6'21](https://youtu.be/jEdgQ-RVmXw?t=381) "So, how do you sort?"*] [*[@9'20](https://youtu.be/jEdgQ-RVmXw?t=560) "The next thing is dates"*] [*[@14'55](https://youtu.be/jEdgQ-RVmXw?t=895) "The way that we get information from dates is using `EXTRACT`"*] [*[@19'55](https://youtu.be/jEdgQ-RVmXw?t=1195) "I need to add this dataset to my kernel"*] [*[@24'10](https://youtu.be/jEdgQ-RVmXw?t=1450) "This is in triple quotation marks because it's actually a string. And BigQuery does expect us to send it a string"*] [*[@25'00](https://youtu.be/jEdgQ-RVmXw?t=1500) "We are going to do a 'safe config'" (re. 1GB of billing quota)*] [*[@26'51](https://youtu.be/jEdgQ-RVmXw?t=1611) "Those are all of the things we are going to talk about today"*] [*[@32'15](https://youtu.be/jEdgQ-RVmXw?t=1935) "And now, within our data, it's sorted first by Quarter ... and then ... by 'number of accidents'. So yes, you can sort by multiple columns"*] [*[@36'16](https://youtu.be/jEdgQ-RVmXw) "So I think it's only going to be from dates" (that `EXTRACT` will work)*] [*[@37'46](https://youtu.be/jEdgQ-RVmXw?t=2266) (re. order you call columns in the query) "`GROUP BY` shouldn't matter, `ORDER BY` should" (...Commutative property, can multiply things in any order)*] [*[@38'31](https://youtu.be/jEdgQ-RVmXw?t=2311) "What is the benefit of using `EXTRACT`, instead of directly `DAY(date)`?" - doesn't work*] [*[@43'55](https://youtu.be/jEdgQ-RVmXw?t=2635) "You don't need to `SELECT` a column, to `GROUP BY` it, **but**..."*] [*[56'16](https://youtu.be/jEdgQ-RVmXw?t=3376) "I think that the problem is that we have a timestamp and not a date"*]

*['Kaggle > Discussion > Learn'](https://www.kaggle.com/learn-forum) for the forum, to ask questions*


## Day 5 (2019-07-17)

"At this point we know quite a few SQL commands. As you write bigger and more complex queries, it becomes more important to break them into small, understandable chunks. Today we’ll learn how to do this using WITH and AS"

* **9. As & With** : [Notebook](https://www.kaggle.com/dansbecker/as-with) with lesson
* **10. As & With** : [Notebook](https://www.kaggle.com/mbeveridge/exercise-as-with/edit) with exercises
* [Livestream (recording 17/7/19)](https://www.youtube.com/watch?v=Hk3OK2G5U5I) (~30min + 30min Q&A) [*[@5'40](https://youtu.be/Hk3OK2G5U5I?t=340) "So that's how `AS` works"*] [*[@6'10](https://youtu.be/Hk3OK2G5U5I?t=370) "But we can also use `WITH` [and `AS`] to refer to a 'CTE' (common table expression) that we have `SELECT` & created" (...but only within scope of that query) (...modular)*] [*[@10'26](https://youtu.be/Hk3OK2G5U5I?t=626) "I see people tend to use single letters for aliasing in this way" ...but I suggest not*] [*[@14'12](https://youtu.be/Hk3OK2G5U5I?t=852) "This query's doing a couple of things, so let's walk through it"*] [*[@21'00](https://youtu.be/Hk3OK2G5U5I?t=1260) "One of the things that I hear a lot, from software engineers, when they're talking about code that they get from data scientists... [be more modular and import from a script]"*] [*[@24'01](https://youtu.be/Hk3OK2G5U5I?t=1441) "Let's ... get questions"*] [*[@30'19](https://youtu.be/Hk3OK2G5U5I?t=1819) "The syntax for multiple `WITH` clauses is..."*] [*[@45'58](https://youtu.be/Hk3OK2G5U5I?t=2758) "The reason why ... this query has problems ... is because here we are not aggregating over everything we select. So let me back up and say what I mean..."*] [*[@55'12-62'00](https://youtu.be/Hk3OK2G5U5I?t=3312) "What if we GROUP by two fields which we know would not return us the same number of groups (eg. days and months)?..."*]

*Rachel's ['With and As Scratchpad'](https://www.kaggle.com/rebeccaturner/with-and-as-scratchpad) kernel, created during Livestream*

*['Kaggle > Discussion > Learn'](https://www.kaggle.com/learn-forum) for the forum, to ask questions*


## Day 6 (2019-07-18)

"We’ve learned a lot about how to get data out of one table in our database… but what about when we want to combine information from more than one table? That’s where joins come in, and that’s what we’ll be going over today"

* **11. Joining Data** : [Notebook](https://www.kaggle.com/dansbecker/joining-data) with lesson
* **12. Joining Data** : [Notebook](https://www.kaggle.com/mbeveridge/exercise-joining-data/edit) with exercises
* [Livestream (recording 18/7/19)](https://www.youtube.com/watch?v=_ERmqiYnrNs) (~30min + 30min Q&A) [*[@3'01](https://youtu.be/_ERmqiYnrNs?t=181) "I was going to show you that in GoogleSheets, you can actually write SQL queries ... (but I think it's going to take too long)"*] [*[3'20-4'10](https://youtu.be/_ERmqiYnrNs) 'super duper fast review'*] [*[@9'37](https://youtu.be/_ERmqiYnrNs?t=577) "So, we want to join these two tables together"*] [*[@19'57](https://youtu.be/_ERmqiYnrNs?t=1197) "And we want to look at the number of files per license..." so will need to `JOIN`*] [*[@24'50](https://youtu.be/_ERmqiYnrNs?t=1490) "And I'm going to just print out the `head` of that dataframe"*] [*[@28'32](https://youtu.be/_ERmqiYnrNs?t=1712) "It is time for questions"*] [*[@38'04](https://youtu.be/_ERmqiYnrNs?t=2284) "This is the order in which they're executed" (not order in which written)*] [*[@39'22](https://youtu.be/_ERmqiYnrNs?t=2362) "So `JOIN` comes 3rd in the execution order"*] [*[55'15](https://youtu.be/_ERmqiYnrNs?t=3315) "Again, I have never heard of 'Junction Tables' before, so that's something for me to research"*] [*[58'11](https://youtu.be/_ERmqiYnrNs?t=3491) "...I don't know the answer. There's a lot of reasons that it could be, and I just don't know"*]

*Rachel's ['Join Scratchpad'](https://www.kaggle.com/rebeccaturner/join-scratchpad) kernel, created during Livestream*

*['Kaggle > Discussion > Learn'](https://www.kaggle.com/learn-forum) for the forum, to ask questions*


## EXTRA: BigQuery ML Workshop (2019-08-07)

"Today we’re going to be training and deploying ML models using BigQuery Machine Learning"

* [Notebook](https://www.kaggle.com/rtatman/bigquery-machine-learning-tutorial) with tutorial
* [Notebook](https://www.kaggle.com/rtatman/bigquery-machine-learning-exercise) with exercises
* [Livestream (recording 7/8/19)](https://www.youtube.com/watch?v=a1onYwwFqj0) (~30min + 30min Q&A) [*[@1'53](https://youtu.be/a1onYwwFqj0?t=113) "Let's call this project 'rachael bqml tutorial'"*] [*[@2'31](https://youtu.be/a1onYwwFqj0?t=151) "And the one I just made isn't showing up, because I haven't got any datasets or models in it yet"*] [*[@2'59](https://youtu.be/a1onYwwFqj0?t=179) "We're ready to start going"*] [*[@3'41](https://youtu.be/a1onYwwFqj0?t=221) "What is BigQuery ML? When should you use it?"*] [*[@7'24](https://youtu.be/a1onYwwFqj0?t=444) "You can upload pre-trained TensorFlow models and then they'll be served from within BigQuery"*] [*[@9'05](https://youtu.be/a1onYwwFqj0?t=546) "The first thing I need to do is link my instance - my project - to my notebook"*] [*[@9'44](https://youtu.be/a1onYwwFqj0?t=584) "We're doing something a little bit different here than we've done previously" (using the notebook magic)*] [*[@10'20](https://youtu.be/a1onYwwFqj0?t=620) "And then you can type SQL directly, without having to put it in the triple quotes, without having to send it to a query object ... This will only work in Jupyter"*] [*[10'54](https://youtu.be/a1onYwwFqj0?t=654) "Today, we are going to be working, for the tutorial, with Google Analytics sample dataset"*] [*[@12'23](https://youtu.be/a1onYwwFqj0?t=743) "And it looks a little bit different ... It's a little bit more complex in terms of data structure"*] [*[@13'36](https://youtu.be/a1onYwwFqj0?t=816) "They are what are called 'structs', or records. So it's basically* **like a JSON file inside a cell**"] [*[@15'08](https://youtu.be/a1onYwwFqj0?t=908) "We'll get the `column name`[`dot`] `the field name we're interested in`"*] [*[@16'06](https://youtu.be/a1onYwwFqj0?t=969) "So,* **we know what the dataset looks like. Now to train a model**"] [*[@16'40](https://youtu.be/a1onYwwFqj0?t=1000) "While it trains, we'll talk about what's in this query. Because this is a big query"*] [*[@19'51](https://youtu.be/a1onYwwFqj0?t=1191) "For logistic regression specifically, if it tries to predict a Null you'll get an error, so we are converting the Nulls to 0"*] [*[@23'02](https://youtu.be/a1onYwwFqj0?t=1382) "This is a complex query ... This is a model that has a fairly large number of things going on in it ... We wanted to show you the range of [options]"*] [*[@23'57](https://youtu.be/a1onYwwFqj0?t=1437) "We've trained our model. Now,* **if you're interested, you can get information on the training statistics**"] [*[@25'24](https://youtu.be/a1onYwwFqj0?t=1524) "So, we didn't have to do a lot, but how did the model do? ... We are going to use this `ML.EVALUATE(MODEL)` function"*] [*[@28'16](https://youtu.be/a1onYwwFqj0?t=1696) "So, this looks pretty good. I'm pretty happy with this"*] [*[@28'44](https://youtu.be/a1onYwwFqj0?t=1724)* "**Can we use it to predict?** *Yes ... It's already in our database, we can just ask for predictions"*] [*[@32'15](https://youtu.be/a1onYwwFqj0?t=1935) "I am going to take questions now"*] [*[@34'58](https://youtu.be/a1onYwwFqj0?t=2098) "How can I send a request to this model from - let's say - a website?"*] [*[37'28](https://youtu.be/a1onYwwFqj0?t=2248) "The reason why you need to link a BigQuery account to do this is because the Kaggle BigQuery account does not have write permissions"*] [*[58'37](https://youtu.be/a1onYwwFqj0?t=3517) "How to run prediction on fresh data?"*]
