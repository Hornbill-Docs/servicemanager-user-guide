---
description: HAi Text Assist is a set of AI-driven tools for the quick creation and manipulation of text content.
coverImage: /_books/servicemanager-user-guide/images/hai-cover.jpg
layout: article-toc
---
# Text assist

Text assist is a collection of AI-powered tools that help you create and edit content quickly. You can use HAi to expand on problems, suggest solutions, check spelling and grammar, or change the tone of your writing. These features are available in text and comment areas through a drop-down menu.

![HAi Text Assist](/_books/servicemanager-user-guide/images/hai-text-assist.png)

## Before you begin

To use HAi services, you must meet the following requirements:

* **Register for the closed beta program**: HAi features are currently in a closed beta. You can access these features after you register. Contact your Hornbill customer success representative to join the program.
* **Review fundamentals**: Read the [HAi fundamentals](/esp-fundamentals/core-capabilities/integration/hai-services) documentation to understand the core concepts.

## Capabilities

You can use Text assist to perform the following actions:

* **Ask HAi**: Enter an open-ended prompt to receive solutions for common issues. For example, "How do I set up an email signature in Outlook?"
* **Change tone**: Adjust the text to suit your audience. Options include:
  * Apologetic
  * Professional
  * Friendly
  * Technical
* **Improve text**: Correct spelling and grammar while improving readability.
* **Shorten text**: Remove unnecessary words to make the content concise.
* **Listify**: Convert blocks of text into a bulleted list.

## Supported areas

You can use Text assist in the following Hornbill record areas:

* Timeline posts
* Documented resolutions
* Email updates
* Bulk update requests from the request list view
* Knowledge articles

## Output formats

Text assist provides content in the format required by the specific text area:

* **Wiki Markup**: Used for timeline updates and request resolutions.
* **HTML**: Used for email updates and knowledge articles.

## Usage tips

### Use snippets for custom prompts

You can combine snippets with request variables and the **Ask HAi** instruction to create custom prompts. For example, use the following snippet to generate an initial response to a user request:

```text
{{summary}}
{{description}}
Write 4 clarifying questions to solve this issue.
```

![Snippet Tip](/_books/servicemanager-user-guide/images/hai-snippet.png)

![Snippet Response](/_books/servicemanager-user-guide/images/hai-snippet-2.png)

### Contextual enrichment

When you use the **Ask HAi** prompt, the system sends additional context from the record to improve the accuracy and relevance of the response.

![Context Tip](/_books/servicemanager-user-guide/images/hai-context.png)
