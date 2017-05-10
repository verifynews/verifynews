---
layout: default
title:  "Final Blog Post"
date:   2017-05-10 03:37:00
categories: main
---
# CrossCheck: Final Blog Post
## Summary of Project

The trustworthiness of any given information on the Web is subjective and hard to capture. Information on the web has traditionally been looked at as an isolated piece of data, but we aim to understand news articles and content in relationship to its existence in relationship to existing content and knowledge. We've created CrossCheck,a content verification algorithm and effort to identify relationships between news articles and illuminate context around an otherwise isolated body of information.   	 

CrossCheck works by consistently sourcing the full text of articles from carefully curated baseline sources and “fake” news sources to our servers. We then extract keywords and a host of other features and train our machine learning algorithms on these sources. Our algorithm includes a logistic regression classifier and on-demand document clustering. The balanced accuracy of the algorithm on a 10-fold cross validation is approximately 94%. Our algorithm rapidly provides: a probability for the accuracy of a body of text, links to related news articles from reputable sources, and a host of other ancillary information.


## What We’ve Accomplished
At the end of Data Science, we've tackled the following tasks
- Created a classifier defined daily/in real time to determine how well a particular body of text or article fits into a web scraped collection of ground/reputable articles. The classifier provides us a likelihood of its belonging.
- Created a document clustering method that provides us insight into the context of any given article
- Explored interesting data relationships informing our decisions in creating our particular clustering and classification techniques
- Built a clean and intuitive Chrome extension/web experience to utilize our algorithm. As any user traverses the web, they see CrossCheck validating articles in the background, and can also view more detailed statistics on demand. The user can also highlight and CrossCheck any particular body of text on demand.

##Conclusions
Have we set out to achieve what we aimed to achieve?

Looking at the goals we set out during our pre-proposal and first blog post, we initially looked to create a broad algorithm to classify news articles. Since then we've worked hard to refine our conception of "truth" and "fake", and established a new concept of "baseline" rather than "truth". We've also honed our algorithm to cater to a much more specific task. Furthermore, we've added ideas and machine learning attempts to provide an actual context for users.

Examining the actual results from our work, we've been highly successful in building a classifier within our testing data. With 10-fold cross validation, our logistic regression has an accuracy of over 94%. Clustering is still a work in progress as we've been able to identify a particular vectorization and clustering method that do capture meaning, but there are also still many unexplained phenomena that need to be ironed out.

We are very proud of our Chrome extension! We really believe that the experience is fast and intuitive. Building and hosting this as a web service as well has been an incredibly rewarding experience.

Thanks so much for this year!
