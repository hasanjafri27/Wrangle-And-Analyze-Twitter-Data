# Wrangle-And-Analyze-Twitter-Data

## Introduction:

This project will be analyzing tweet archive of Twitter user @dog_Rates (A.K.A. WeRateDogs) that rates and comments on people's dogs. Data gather from real world always isn't clean. Python libraries are used to gather, assess and clean its quality/tidyness.

## Steps/Tasks:

1. Gathering 3 datasets
2. Assessing data for quality and tidiness issues
3. Cleaning data for all issues
4. Insights & visualization

### 1. Gathering Data:

Twitter_archive_enhanced: Provides each tweet that includes dog name, dog score and dog stage. This link is provided to download manually.

Tweet image predictions data (what breed of dogs): Classify each tweet's dog breeds according to a neural network. This file (image_predictions.tsv) can be downloaded programmatically from Udacity's servers using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

Twitter API & JSON: Include retweet count and favorite count will be gathered using Tweepy to query Twitter's API for additional data beyond the data included in the WeRateDogs Twitter archive.

### 2. Assessing Data:

Both visual and programatic assessments were done to point out quality and tidiness issues. Quality issues are content issues that is inaccurate or redundant. Tidiness issues are the structural issues and unorganized data frames.

#### Quality Issues:

1. Retweets are inlcuded in the dataset.
2. Data contains unnecessary columns.
3. Invalid values in numerators and denominators.
4. Retweeted_status_timestamp, timestamp should be datetime instead of strings.
5. Duplicates in jpg_url.
6. Inconsistent capital words/letter in p1, p2 and p3.
7. Underscores in p1, p2, and p3.
8. Three columns dedicated for p1, p2 and p3 instead of one.
9. Rename id to tweet_id.

#### Tidiness Issues:

1. Tweet_ids of type integar in all of the tables.
2. Four columns dedicated for stages of dogs(doggo floofer pupper puppo) instead of one.
3. Data divided between 3 datasets instead of one.

### 3. Cleaning Data:

Cleaning were performed on every issues found on assessment step. Each issue is fixed by the following 3 steps:

Define: Explaining the problem and the approach. Code: The complete code that run to fix the data. Test: Assess the data again to make sure the code works and fixed the issue.

### Conclusion:

By wrangling the Twitter datasets with many Python libraries with above 3 steps. The datasets became much cleaner. The datasets are now ready to be analyzes to find meaningful insights, then build visualization to summarize the results.
