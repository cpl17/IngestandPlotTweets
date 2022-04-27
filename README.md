This project contains the following:

* A short script that utilizes Tweepy and Twitter dev API to locally serve tweets
* The tweets are filtered according to a provided keyword
* Concurrently, a spark app is hosted on the same port and ingests the tweets every 10 seconds
* Then, a MapReduce operation is performed on the RDDs to find the hashtag frequencies, which are stored in a temporary table
* The top 10 hashtags are queried using SparkSQL
* Finally, a dynamic bar plot of the frequencies is created

