# Fake-News-Detection

Fake news detection has recently attracted a growing interest from the general public and researchers as the circulation of misinformation online increases, particularly in media outlets such as social media feeds, news blogs, and online newspapers. For instance, a recent report by the Jumpshot Tech Blog1 found that Facebook referrals accounted for 50% of the total traffic to fake news sites and 20% total traffic to reputable websites. In the field of Fake News Detection, a lot depends on the common features extracted from the corpora. Hence, it’s easy to see why Domain-dependant fake news detection would be a manageable task - since feature learning would be a relatively easy task. However, domain invariant fake news detection would be a significantly more difficult task as it involves learning of features that span over news from multiple domains.

## Dataset Used:

Data scraping (both Real and Fake) was done with Selenium Web Browser Automation. The script written uses Selenium to crawl over all the links present in the url and extract Heading and Data part of it. Sources for the Fake news includes data from fakingnews.com, beforeitsnews.com, worldnewsdailyreport.com and for the Real news bbc.com, news.google.com, news18.com. Five categories of each fake and real news were extracted.The categories includes "India", "Politics", "Entertainment", "Sports", "Technology".

## Model

We have used an LSTM based model by taking GloVe feature vectors for word embedding. We conduct several experiments with different combinations of hyper-parameters. We have used binary cross entropy loss with Adam optimizer setting learning rate as 0.001 with a decay of 0.1. We ran it for 10 epochs with batch size 32. We have used ReLU activation function for LSTM and dense layers. Total 5,801,697 parameters has been trained. Model architecture has shown below.
