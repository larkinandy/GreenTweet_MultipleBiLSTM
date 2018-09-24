# GreenTweet_MultivariateBiLSTM: Data Collection
text and metadata collection from twitter

**Author:** Andrew Larkin <br>
**Affiliation:** Oregon State University, College of Public Health and Human Sciences <br>
**Date Created:** September 23rd, 2018

**Summary:** <br>
In a [previous study](https://github.com/larkinandy/Portland_UrbanNature_Twitter), we collected tweets related to urban nature from January 1st, to December 31st, 2017.  This document briefly summaries the methodologies and results. See external links below for more details.

This document contains the following sections:
1) **Previous study** - brief description of previous study for which the twitter dataset was collected
2) **Scripts** - custom derived scripts used to download database
3) **External links** - hyperlinks to previous study github and libraries used for data collection

**TODO:**
- [ ] add citation to previous study once published

### Previous study ###
In a [previous study](https://github.com/larkinandy/Portland_UrbanNature_Twitter), we downloaded tweets from the twitter API stream from January 1st, 2017 to December 31st, 2018 that contained the following keywords:

Keywords 1-5 | Keywords 6-10 | Keywords 11-15 | Keywords 16-20 | Keywords 21-25
------------ | ------------- | ------------- | ------------- | -------------
backyard | forest | lawn | pasture | stream |
bush |  garden | leaf | plant | trail |
crop | grass | mountain | prarie | tree |
field | hay | nature | river | wood |
flower | lake | park | riverside | yard |


**Table 1.  Search keywords used to download tweets from the Twitter Stream API.** Table 1 shows only singular keywords.  However, both singular (e.g. leaf) and plural (e.g. leaves) forms of the keywords were downloaded.

Data were stored in a mySQL database. Primary key consisted of a unique incremental integer.  

### Scripts ###
Scripts were written in python and use the tweepy pacakge.

**TODO:**
- [ ] add script names and brief description.

### External links ###
- **Previous study github repository** - https://github.com/larkinandy/Portland_UrbanNature_Twitter
- **Tweepy** - http://www.tweepy.org/
- **mySQL Workbench** - https://www.mysql.com/products/workbench/
