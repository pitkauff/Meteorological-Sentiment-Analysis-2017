# Twitter Sentiment Analysis

This project was part of COMS 6998 - Projects in Data Sciene at Columbia.

**Problem Statement**

The purpose of this project was to apply some form of machine learning on streaming data. We decided to investigate whether or not weather patterns have any influence on overall social media sentiment, as expressed through Twitter and Buzzfeed.

**How to use this code**

CHANGE YOUR PYTHONPATH
We ran this project through PyCharm, which uses absolute paths from the root directory of our project.
In order for the code to run at all outside of PyCharm run the following command:
export PYTHONPATH="${PYTHONPATH}:/<path_to_project_root>


____________
Collect
____________

To collect twitter data we used the saveTweets function in twitterAPI.py

An example of this can be found in twitter/denver.py
(Information on the places we used can be found in data/places.json)

____________

To collect Reddit data, we used the timesearch.py script.
In terminal, run the following two commands sequentially (as example)

python timesearch.py timesearch -r denver
python timesearch.py commentaugment -r denver

This will create a sqlite DB. You can use sqlite browser to read then export this to a csv.

___________
Enrich
___________

To enrich data we used the enrichAllPlaces function in enrich/enrichData.py
(EnrichRedditData function for reddit data)

___________
Learn
___________

To run our regressors we used the functions in learn/machineLearning.py
An example of this can be found in learn/randomForest.py
