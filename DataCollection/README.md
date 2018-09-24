# GreenTweet_MultivariateBiLSTM: Data Collection
text and metadata collection from twitter

**Author: ** Andrew Larkin
**Affiliation:** Oregon State University, College of Public Health and Human Sciences
**Date Created:** September 23rd, 2018

**Summary** <br>
In a previous study, we collected tweets related to urban nature from January 1st, to December 31st, 2017.  This document briefly summaries the methodologies and results.  For more details, please see the corresponding github repository at: https://github.com/larkinandy/Portland_UrbanNature_Twitter
This document contains the following sections:
1) **Previous study** - brief description of previous study for which the twitter dataset was collected
2) **Scripts** - custom derived scripts used to download database
3) **External links** - hyperlinks to previous study github and libraries used for data collection

**TODO: **
- [ ] add citation to previous study once published
- [ ] add hyperlink to tweepy library
- [ ] add tweepy and python versions


### Previous study ###
In a previous study, we downloaded tweets from the twitter API stream from January 1st, 2017 to December 31st, 2018 that contained the following keywords:

Search Keyword | 
------------ |
backyard | 
bush | 
crop
field
flower
forest
garden
grass
hay
lake
lawn
leaf
mountain
nature
park
pasture
plant
prarie
river
riverside
stream
trail
tree
wood
yard

** Table 1.  Search keywords used to download tweets from the Twitter Stream API**

Data were stored in a mySQL database. Primary key consisted of a unique incremental integer.  

### Scripts ###
Scripts were written in python and use the tweepy pacakge.

### Externa links **
- **Previous study github repository **
- **Tweepy** 
- **mySQL Workspace**
