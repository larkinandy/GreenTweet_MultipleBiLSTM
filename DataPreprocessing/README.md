# GreenTweet_MultivariateBiLSTM: Data Preprocessing
text and metadata collection from twitter




 **Dataset** | Train | Dev | Test |All | Train | Dev | Test | All 
 ------------ | ------------- | ------------- | ------------- | ------------- | ------------- | ------------ | ------------- | ------------ 
**Nature Label** |1|1|1|1|0|0|0|0|
**Sample Size** | 36654 | 2897 | 2981 | 42532 | 26309 | 2103 | 2019 | 30341 
**Label Frequency (%)** |  --------- | --------- | --------- | --------- | --------- | -------- | --------- | -------- 
&nbsp;&nbsp;&nbsp;&nbsp; Safety | 6.96 | 6.97 | 5.77 | 6.87 | 2.35 | 2.43 | 2.23 |2.34 |
&nbsp;&nbsp;&nbsp;&nbsp; Beauty | 6.35 | 6.80 | 5.90 | 6.35 | 0.94 | 1.14 | 1.19 | 0.97 |
&nbsp;&nbsp;&nbsp;&nbsp; Social | 13.04 | 13.32 | 13.45 | 13.08 | 5.23 | 4.52 | 5.05 | 5.18 |
&nbsp;&nbsp;&nbsp;&nbsp; Stress | 1.38 | 1.50 | 1.17 | 1.37 | 0.35 | 0.43 | 0.50 | 0.36 |
&nbsp;&nbsp;&nbsp;&nbsp; Air | 1.06 | 1.04 | 1.24 | 1.07 | 0.20 | 0.38 | 0.01 | 0.20 |
**Emoticon Frequency (%)** | 10.02 | 10.25 | 11.64 | 10.15 | 5.93 | 6.09 | 6.29 | 5.96 |
**Hashtag Frequency (%)** | 23.92 | 24.17 | 24.89 | 24.01 | 18.12 | 18.69 | 16.94 | 18.08 |
**Mean Sentence Length (words)** | 18.42 | 18.63 | 18.78 | 18.46 | 19.65 | 19.84 | 19.47 | 19.65 |

**Table 1.  Select Descriptive Statistics from the Train, Test, and Dev Datasets Created from the Data Preprocessing Script, Stratified by Nature Class (1 = positive, 0 = negative)**. <br> <br> <br>





**Author:** [Andrew Larkin](https://www.linkedin.com/in/andrew-larkin-525ba3b5/) <br>
**Affiliation:** [Oregon State University, College of Public Health and Human Sciences](https://health.oregonstate.edu/) <br>
**Date Created:** September 26th, 2018 <br>

**TODO:** <br>
[ ] add link to POS paper once it's available online <br>

**Summary** <br>
Data Preprocessing for the bi-LSTM requires several NLP modifications that weren't required for the [previous Twitter analysis based on Part of Speech tagging](https://github.com/larkinandy/Portland_UrbanNature_Twitter).  Most notably:
- a mapping dictionary needs to be made to transform tweet text into word vectors <br>
- unknown and padding tags need to be added to sentences <br>
- sentence length prior to adding padding needs to be determined <br>
- ompatected words need to be partitioned into multiple words (e.g. #lastchildinthewoods) <br>
- indicators need to be made to indicate which words in the text belong to hashtags and emoji descriptions <br>
- inclusion criteria need to be applied to limit bayes optimal error arising from ambiguous text <br>
- the dataset needs to be partitioned into train, dev, and test sets <br>
- descriptive statistics need to be run to compare train, dev, and test set compatibility <br>

The Data Preprocessing section contains the following documents:
- [**DatasetDescriptiveStats.xlsx**](./DatasetDescriptiveStats.xlsx) - Table with descriptive statistics for train, test, and dev datasets
- [**PreprocessTweets.ipynb**](./PreprocessTweets.ipynb) - Jupyter notebook containing python script for performing all of the operations described above <br>
- [**AddRegionalContextIndicator.ipynb**](./AddRegionalContextIndicator.ipynb) - Jupyter notebook for adding the regional contet flag - indicates whether a word within the tweet text corresponds to a keyphrase that has unique context within the originating region <br>
- **Readme.md** - this file, documenting the precprocess workflow and results

**External Links** <br>
**Stanford Word Vectors** - https://nlp.stanford.edu/projects/glove/ <br>



![alt text](https://raw.githubusercontent.com/larkinandy/GreenTweet_MultivariateBiLSTM/master/DataPreprocessing/images/preProcessingWorkflow.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Figure 1.  Workflow Diagram for Data Preprocessing.** <br>
