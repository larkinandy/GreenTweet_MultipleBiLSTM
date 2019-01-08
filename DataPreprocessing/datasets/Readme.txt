These datasets were used to train and test the Green Tweet biLSTM model.  
To fit in the git repository, datasets are zipped and pickled.  
The test and NYC datasets are currently available.  
The dev set will be added after the manuscript is published.  
The train dataset may be added later, depending on repository size limitationss.  

Dictionary keys in each datase are:
sent - tweet sentences
labels - coded labels in the following order: greenspace, safety, beauty, exercise, social, stress, air
hash - hashtag indicator for each word in a tweet
emot - emoticon indicator for each word in a tweet
loc - reigonal context indicator for each word in a tweet
seqLens - length of words in tweet before pad tokens
