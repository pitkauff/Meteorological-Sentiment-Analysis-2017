# Twitter Sentiment Analysis

This project was part of COMS 6998 - Projects in Data Sciene at Columbia.

**Problem Statement**

The purpose of this project was to apply some form of machine learning on streaming data. We decided to investigate whether or not weather patterns have any influence on overall social media sentiment, as expressed through Twitter and Buzzfeed.

**How to use this code**

Change your PYTHONPATH. We ran this project through PyCharm, which uses absolute paths from the root directory of our project.
In order for the code to run at all outside of PyCharm run the following command:

    export PYTHONPATH="${PYTHONPATH}:/<path_to_project_root>

**Script Overview**

- [Collect](https://github.com/pitkauff/Meteorological-Sentiment-Analysis-2017/tree/master/scripts/collect): These scripts were used to stream live tweets and save them to a mongodb database using the [pymongo API](https://api.mongodb.com/python/current/).
- [RedditSearch](https://github.com/pitkauff/Meteorological-Sentiment-Analysis-2017/tree/master/scripts/redditSearch): These scripts were used to stream reddit data.
- [Enrich](https://github.com/pitkauff/Meteorological-Sentiment-Analysis-2017/blob/master/scripts/enrich/enrichData.py): This script was used to add weather and sentiment to the twitter / Reddit data.
- [Learn](https://github.com/pitkauff/Meteorological-Sentiment-Analysis-2017/tree/master/scripts/learn): This folder includes all regression algorithms that were used in order to predict sentiment based on weather data.
