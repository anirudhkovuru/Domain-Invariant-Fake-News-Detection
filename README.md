# Fake-News-Detection

Fake news detection has recently attracted a growing interest from the general public and researchers as the circulation of misinformation online increases, particularly in media outlets such as social media feeds, news blogs, and online newspapers. For instance, a recent report by the Jumpshot Tech Blog1 found that Facebook referrals accounted for 50\% of the total traffic to fake news sites and 20\% total traffic to reputable websites. In the field of Fake News Detection, a lot depends on the common features extracted from the corpora. Hence, it’s easy to see why Domain-dependant fake news detection would be a manageable task - since feature learning would be a relatively easy task. However, domain invariant fake news detection would be a significantly more difficult task as it involves learning of features that span over news from multiple domains.

## Dataset Used:

We scraped the fake data from [Faking News](fakingnews.com) of various categories which is as follows
  - India,
  - Politics,
  - Entertainment,
  - Technology
We have a total of 299 samples of both real and fake news.

## Model

We have trained an LSTM model followed by dense layer. GloVe embedding of 300 dimensions has been used. RMSProp Optimizer is used with binary cross entropy loss. We ran it for 10 epochs.
