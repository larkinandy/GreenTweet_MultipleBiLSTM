# GreenTweet_MultivariateBiLSTM
twitter text preprocessing and bidirectional lstm for multivariate categorization

## Public visibility for this project is limited until manuscript has been accepted for publication ## 

**Author:** [Andrew Larkin](https://www.linkedin.com/in/andrew-larkin-525ba3b5/) <br>
**Affiliation:** [Oregon State University, College of Public Health and Human Sciences](https://health.oregonstate.edu/) <br>
**Date Created:** September 23rd, 2018 <br>

**Summary** <br>
The purpose of this project is to download text from twitter posts related to urban nature, or "greenspace", preprocess the text for developing classifiers, create a multivariate classifier for greenspace related pathways of action, and evaluate model performance.  Github contents are partitioned into the following folders:

1) **Documentation** - background information, project purpose, project description, and data sources. <br>
2) [**Data Collection**](DataCollection) - scripts used to download data from Twitter and store in SQL database, along with results
3) **Data Preprocessing** - NLP scripts to screen, clean, and standardize tweet text and metadata, along with results
4) **Model Training and testing** - Tensorflow scripts for training and testing rnn models, along with results
5) **Model Validation** - Tensorflow scripts for model validation, along with results
