---
title: Hornbill AI - Sentiment Analysis
description: HAi Sentiment Analysis will analyze the sentiment of a request/ticket at the click of a button. One fewer task for your agents.
coverImage: /_books/servicemanager-user-guide/images/hai-cover.jpg
layout: article-toc
---

# Sentiment Analysis
Analysise the sentiment of a request/ticket at the click of a button. One fewer task for your agents.

### Benefits to you
* Instantly analyze the sentiment of a customer on a request
* Audited over the lifespan of the request

### What you can do
* One-click Sentiment Analysis of ticket details and actions.

### Where to find it
In any request record, you'll see the new HAi Overview box. Simply click the HAi icon on the right-hand side to generate the request overview including the sentiment.
<img src="/_books/servicemanager-user-guide/images/hai-logo-small.png" alt="Hornbill Ai" width="50px"></img>

### How to use it

1.
    Open a request record. Go to the *HAi Overview* area and click the HAi icon.
    <img src="/_books/servicemanager-user-guide/images/hai-sentiment-analysis-1.png" alt="Hornbill Sentiment Analysis"></img>

2.
    HAi generates the sentiment and automatically saves it, this value is audited for reporting on at a later stage
    <img src="/_books/servicemanager-user-guide/images/hai-sentiment-analysis-2.png" alt="Hornbill Sentiment Analysis"></img>


### Template Variables
Request Sentiment can be used in email templates as the variable is available with the others.
<img src="/_books/servicemanager-user-guide/images/hai-sentiment-analysis-3.png" alt="Hornbill Sentiment Analysis - Email"></img>

### Auto Updates
Its possible to enable [auto updates](/servicemanager-config/administration/hai-request-summariser) for Sentiment Analysis

### Request Insights
Once a request is resolved or closed, the request insights tab can be used to show reports on the history of the sentiment against a given request over time.

### Sentiment Values

Sentiment value stored in the database and available in template variables has the follow corosponding labels

| Sentiment Value  	| Sentiment Label  	| 
|---	            |---	            |
| 0  	            | No Sentimetn Found| 
| 1  	            | Most UnHappy      |
| 2 	            | UnHappy           |
| 3  	            | Neutral           | 
| 4  	            | Happy  	        |
| 5 	            | Most Happy        |