# Udacity-DataAnalystND-P2-Wrangle-and-Analyze-Data

# Project 2: Wrangle and Analyze Data

Gather data from a variety of sources and in a variety of formats, assess its quality and tidiness, then clean it. Showcase your wrangling efforts through analyses and visualizations.

## Introduction
Real-world data rarely comes clean. Using Python and its libraries, you will gather data from a variety of sources and in a variety of formats, assess its quality and tidiness, then clean it. This is called data wrangling. You will document your wrangling efforts in a Jupyter Notebook, plus showcase them through analyses and visualizations using Python (and its libraries) and/or SQL.

The dataset that you will be wrangling (and analyzing and visualizing) is the tweet archive of Twitter user [@dog_rates](twitter.com/dog_rates) , also known as [WeRateDogs](https://en.wikipedia.org/wiki/WeRateDogs). WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because ["they're good dogs Brent."](http://knowyourmeme.com/memes/theyre-good-dogs-brent) WeRateDogs has over 4 million followers and has received international media coverage.

WeRateDogs [downloaded their Twitter archive](https://support.twitter.com/articles/20170160) and sent it to Udacity via email exclusively for you to use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017. More on this soon.

## Report: act_report

### Insight 1.There are more tweets from Iphone than other platforms.
We notcied that the most used platform for tweets is **Iphone** and there is an explanation for this: @WeRateDogs account is located in United States of America and the first audience of accounts are the most closest community. We can say that the account has been followed by many americans first before expanding to other countries. The **Apple, Inc** company has conquered the local market, means that most americans users have an Iphone.

### Insight 2.The most used rating numerator note is `12`.
Most the dogs are rated 12. Looks like `There are good dogs` more than we can ever imagine. Even though there are rating notes under 10, we can argue that our wrangling efforts have not been made without errors because *"the rating numerators are greater than the denominators does not need to be cleaned. This [unique rating system](http://knowyourmeme.com/memes/theyre-good-dogs-brent) is a big part of the popularity of WeRateDogs."* So it can be considered as error every rating numerator under 10. Hopefully, these errors aren't many and we could process our analysis without big troubles. 

### Insight 3.There is a high correlation between `retweet_count` and `favorite_count`
We noticed in our analysing effortsthat there is a high correlation between `retweet_count` and `favorite_count` over `0.90`. This means that the more an tweet is retweeted, the more it can get liked as `favorite` because when someone retweet, it makes the tweet available for his audience and most of his audience like it and retweet it again and aigain and so on.