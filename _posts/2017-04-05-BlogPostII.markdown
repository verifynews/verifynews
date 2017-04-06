---
layout: default
title:  "Verifying News: Blog Post II"
date:   2017-04-05 20:04:00
categories: main
---
# Verifying News: Midterm Blog

# Technical Overview

## Relational SQL Database & Apache Tomcat Server

Every 5 minutes, our script in Java queries all news articles published from the top news sources using
webhose.io. These news articles including a host of ancillary information (see Database Schema Design)
and the information is efficiently saved to the Microsoft SQL Server hosted on Azure. We use an
asynchronous multithreaded approach to maximize efficiency and effective parallelization. The code
runs as an Apache Tomcat Webapp on Microsoft’s Azure server.

## Django Server
The Django server is the brain of the backend. Processing user requests as a URL, retrieving information from webhose.io corresponding to that URL and running the information through the algorithm. The backend can easily scale to support milliosn of clients and interfaces seamlessly with our SQL Server. The Django server is also responsible for periodically querying the SQL Server and pre-computing the clusters/category that are used in the algorithm. 

## Technologies we're using
Technologies we're using: Django webframe, Microsoft SQL Server, Apache Tomcat

## Visualizations
![News Verification Visualization 1]({{ site.url }}/verifynews/assets/59A373AF-0BE9-4549-B272-E93EBC44A506.png)

![News Verification Visualization 2]({{ site.url }}/verifynews/assets/0968D4A8-E3FA-4FCE-A73C-3FB26281F65A.png)

![News Verification Visualization 3]({{ site.url }}/verifynews/assets/489200C6-5AC4-4400-AE45-BEB8696BBB29.png)

![News Verification Visualization 4]({{ site.url }}/verifynews/assets/A2FBEB89-7CF6-4E99-8A93-79F6CA00725C.png)
## Concrete results
We have tens of thousands of news articles, information fully parsed, stored in our cloud-based databases. We've yet to perfect and run our algorithm, but the data is there and ready to be analyzed

## Biggest problems we're facing
Biggest problem? No doubt optimizing our algorithm to handle every imaginable news source and edge case: local news sources, fresh news sources, little-known news sources, sources with poor grammar, sources with unconventional writing styles/diction

## Initial Insights

Our initial insights: fake news verification is an incredibly touchy subject. It is literally impossible to please everyone. We're hoping, however, that we can show our audience that our approach is sufficiently unbiased so as to please liberals and conservatives alike. Further, there's just so much junk data when you're crawling in massive volumes. Most won't notice if a single news article in a hundred turns out completely bogus in our databases, but when you have on the order of tens of thousands, these things really rack up errors. 

## Are we on track?
We are absolutely on track with the project. We're now proceeding on creating the Django webserver.


## Going forward?
Given the initial results, even from our rough-draft algorithm, the results are incredibly promising. We've far exceeded the >70% threshold we were looking for. Things can only improve as we seek more advice on the algorithmic approach from professors and finetune our machine learning model. 
