# GreenTweet_MultivariateBiLSTM: Data Preprocessing
text and metadata collection from twitter

**Author:** [Andrew Larkin](https://www.linkedin.com/in/andrew-larkin-525ba3b5/) <br>
**Affiliation:** [Oregon State University, College of Public Health and Human Sciences](https://health.oregonstate.edu/) <br>
**Date Created:** September 26th, 2018 <br>

**TODO:** <br>
[ ] add link to Stanford word vector model <br>
[ ] add link to related repository <br>
[ ] add link to POS paper once it's available online <br>
[ ] add select descriptive statistics table <br>
[ ] add pipeline diagram and brief explanation <br>
[ ] fix link to xls file <br>

**Summary**
Data Preprocessing for the bi-LSTM requires several NLP modifications that weren't required for the previous analysis based on Part of Speech tagging (insert link to repository).  Most notably:
- A mapping dictionary needs to be made to transform tweet text into word vectors <br>
- Unknown and padding tags need to be added to sentences <br>
- sentence length prior to adding padding needs to be determined <br>
- compatected words need to be partitioned into multiple words (e.g. #lastchildinthewoods) <br>
- indicators need to be made to indicate which words in the text belong to hashtags and emoji descriptions <br>
- inclusion criteria need to be applied to limit bayes optimal error arising from ambiguous text <br>
- the dataset needs to be partitioned into train, dev, and test sets <br>
- descriptive statistics need to be run to compare train, dev, and test set compatibility <br>

The Data Preprocessing section contains three documents:
1) [**DatasetDescriptiveStats.xlsx*](./DatasetDescriptiveStats.xlsx) - Table with descriptive statistics for train, test, and dev datasets
2) [**PreprocessTweets.ipynb**](./PreprocessTweets.ipynb) - Jupyter notebook containing python script for performing all of the operations described above <br>
3) **Readme.md** - this file, documenting the precprocess workflow and results

**External Links** <br>
insert link to stanford word vector model here <br>

