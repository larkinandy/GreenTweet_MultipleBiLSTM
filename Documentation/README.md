# GreenTweet_MultivariateBiLSTM: Documentation
text and metadata collection from twitter

**Author:** [Andrew Larkin](https://www.linkedin.com/in/andrew-larkin-525ba3b5/) <br>
**Affiliation:** [Oregon State University, College of Public Health and Human Sciences](https://health.oregonstate.edu/) <br>
**Date Created:** September 26th, 2018 <br>

This document is divided into four sections: background, project purpose, project descrption, and external sources.

### Background ###

Urban nature is associated with many positive health outcomees, including reduced stress, blood pressure, rates of depression, and increased levels of exercise, attention restoration, social cohesion, and birth wegiht.  While this exposure-outcome relationship is well established, the speciic pathways of action, interactions between pathways, and tmeporal variation in pathways of action are still uncertain.  

Social media is a context rich and temporally frequent data source which contains significant potential for quantifying the pathways through which people utilize urban nature.  In a [previous study](https://github.com/larkinandy/Portland_UrbanNature_Twitter), we developed latent constructs for these pathways using part of speech tagging.  However, sensitivity analyses found that a POS, while more accurate than a simple frequency-based appraoch, still produced significant levels of construct misclassification.  

### Project Purpose ###

The purpose of this project is to predict whether tweets belong to one or more of seven latent constructs based on content within the tweet.  If the developed model meets accruacy requirements, then it will be impelemente in an automated pipeline to predict latent constructs for 500 cities in the United States in real time.

### Project Description ###

The following are the latent constructs the model will be developed to predict <br>
1) **Greenspace** - whether a tweet contains content relevant to urban nature <br>
2) **Safety** - whether a tweet mentions or is related to safety (either inreased or decreased) <br>
3) **Exercise** - whether tweet mentions some form of exercise, including walking, running, and kayaking <br>
4) **Beauty** - whether tweet describes an aesthetic quality (either positive or negative) <br>
5) **Social** - whether a tweet is relevant to social cohesion, including social groups and/or social events <br>
6) **Stress** - whether a tweet describes an increase or descrease in stress level and/or attention restoration <br>
7) **Air** - whether a tweet describes air quality <br>

We [previously downloaded](https://github.com/larkinandy/Portland_UrbanNature_Twitter) one year of tweets from the Portland, OR metrpolitan region. To prepare these tweets for machine learning, the lead author coded these tweets for all 7 of the latent constructs. We will then perform [additional preprocessing](https://github.com/larkinandy/GreenTweet_MultivariateBiLSTM/tree/master/DataPreprocessing) using the python NLTK package, and then [create a bidirectional LSTM model](https://github.com/larkinandy/GreenTweet_MultivariateBiLSTM/tree/master/ModelTrainingAndTesting) to predict whether a tweet is related to one or more of the seven latent constructs. Finally, [validation studies](https://github.com/larkinandy/GreenTweet_MultivariateBiLSTM/tree/master/ModelValidation) will demonstrate model efficacy, and for which latent constructs model predictions are accurate enough to use in an automated pipeline. <br>

### External Sources ###

**TODO: 

[  ] - add reference to Portland urban nature paper once published

1) Tweepy - http://www.tweepy.org/
2) NLTK - https://www.nltk.org/
3) Greeness and Health - https://health.oregonstate.edu/labs/spatial-health/research/greenness-and-health
