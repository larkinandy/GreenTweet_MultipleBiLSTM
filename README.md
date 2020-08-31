# GreenTweet_MultivariateBiLSTM
twitter text preprocessing and bidirectional lstm for multivariate categorization

**Author:** [Andrew Larkin](https://www.linkedin.com/in/andrew-larkin-525ba3b5/) <br>
**Affiliation:** [Oregon State University, College of Public Health and Human Sciences](https://health.oregonstate.edu/) <br>
**Date Created:** September 23rd, 2018 <br>

**Summary** <br>
The purpose of this project is to download text from twitter posts related to urban nature, or "greenspace", preprocess the text for developing classifiers, create a multivariate classifier for greenspace related pathways of action, and evaluate model performance.  Github contents are partitioned into the following folders:

1) [**Documentation**](Documentation) - background information, project purpose, project description, and data sources. <br>
2) [**Data Collection**](DataCollection) - scripts used to download data from Twitter and store in SQL database, along with results
3) [**Data Preprocessing**](DataPreprocessing) - NLP scripts to screen, clean, and standardize tweet text and metadata, along with results
4) [**Model Training**](ModelTraining) - Tensorflow scripts for training models, including hyperparamter tuning
5) [**Model Evaluation**](ModelEvaluation) - Tensorflow scripts for model evaluation, along with performance results

**Referenes** <br>
1) Andrew Larkin, Perry Hystad, Integrating Geospatial Data and Social Media in Bidirectional Long-Short Term Memory Models to Capture Human Nature Interactions, The Computer Journal, , bxaa094, https://doi.org/10.1093/comjnl/bxaa094
