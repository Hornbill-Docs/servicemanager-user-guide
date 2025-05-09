---
title: Hornbill AI - Text Assist
description: HAi Text Assist is a set of AI-driven tools for the quick creation and manipulation of text content.
coverImage: /_books/servicemanager-user-guide/images/hai-cover.jpg
layout: article-toc
---
# Text Assist

A set of AI-driven tools for quick creation and manipulation of text content. Ask HAi to elaborate on a problem, suggest a solution, spell check and grammar check content, shorten, listify, or change the tone. These features are available anywhere you can post text or comments - accessible from a simple drop-down menu.

![Hornbill AI Dashboard](/_books/servicemanager-user-guide/images/hai-text-assist.png)

## What you can do

* Ask HAi - An open-ended prompt for getting how-to solutions to common issues - for example "How to set up an email signature in Outlook in Office 365".
* Change the tone of the text in the box to suit the audience:
  * Apologetic
  * Professional
  * Friendly
  * Technical
* Improve Text - Correct spelling, and grammar, and improve readability/clarity.
* Shorten Text - Remove unnecessary words.
* Listify - Restructure the content in the box in list form rather than blocks of text.

## Where you can use it

Text areas within Hornbill records:

* Adding a post to a request timeline
* Adding a documented resolution to a request
* Writing an email update to the customer
Bulk update requests from the request list view
* Knowledge articles

## Output format

Text Assist returns content in the format that the text area uses. For example, when updating a timeline or resolving a request, it will return Wiki Markup. When adding an email update or knowledge, it will output HTML.

### Tips and Tricks

1. Snippets - You can use snippets with request variables and the Ask HAi instruction to store custom prompts, one example is to use the following snippet for producing an initial response to a user's request.

  ```TEXT
  {{summary}}
  {{description}}
  Write 4 clarifying question to solve this issue.
  ```

![Snippet Tip](/_books/servicemanager-user-guide/images/hai-snippet.png)
![Snippet Response](/_books/servicemanager-user-guide/images/hai-snippet-2.png)

2. Ask HAi prompt is sent as additional context to enrich the response.

![Context Tip](/_books/servicemanager-user-guide/images/hai-context.png)