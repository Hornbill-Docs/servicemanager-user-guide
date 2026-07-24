# Searching for Requests

## Global search for requests

The **Global Search for Requests** allows you to quickly locate Service Manager requests, including Incidents, Service Requests, Problems, Changes, Known Errors and Releases.

![Global Search bar](/_books/servicemanager-user-guide/request-list/images/global-search-for-requests.png)

The Requests search option is available from the platform's Global Search when Service Manager is installed. It is only visible to users who have permission to use Service Manager.

### Search bar

The search is a natural language search where you can type anything from a single word to a sentence into the search bar. The text typed into the search bar will search the following fields of a request:

* Request ID
* Summary
* Description
* External Reference Number

## Search tools

Search tools are available from the arrow on the right-hand side of the Global Search field. These filters help narrow the search results before the search is performed.

| Filter | Description |
| --- | --- |
| **Any Type** | Limits results to a specific request type including Incident, Service Request, Change, Problem, Known Error and Release. |
| **Any Status** | Filters requests by status including New, Open, On Hold, Resolved, Closed and Canceled. |
| **Any Owner** | Returns only requests owned by the selected co-worker. |
| **Any Customer** | Returns only requests where the selected customer (contact, co-worker or basic user) is the customer of the request. |
| **Any Service** | Limits the search to requests belonging to a selected service. |
| **Details** | Searches Request ID, Summary, Description and External Reference Number. |
| **Timeline** | Searches request timeline entries. |
| **Historic Updates** | Searches historic updates imported from Hornbill Supportworks. This option is displayed only when historic request data exists. |

> **Note**: The **Historic Updates** option is displayed only when historic request data has been imported into Service Manager.

## Search results

Search results are displayed in pages. Depending on the selected search type, results are presented differently.

### Details search results

The Details search displays:

* Request ID
* Summary
* Logged Date
* Status
* Owner
* Customer
* Team
* Service
* External Reference Number (when available)

Users with permission to view a request can open it directly from the search results.

### Timeline search results

The Timeline search displays:

* Request ID
* Matching timeline content
* Published Date
* User who created the timeline entry

Each result includes an **Open Post** button that opens the original timeline entry within the request.

### Historic updates search results

The Historic Updates search displays:

* Request ID
* Matching historic update content
* Updated Date
* User who performed the update

> **Note**: Historic Updates are read-only records imported from Hornbill Supportworks.

## Ordering search results

Results can be reordered using the **Order By** drop-down. The available options depend on the selected search type.

### Details ordering

* Relevance (default)
* Logged Date (Newest)
* Logged Date (Oldest)
* Last Modified (Newest)
* Last Modified (Oldest)

### Timeline ordering

* Relevance (default)
* Published Date (Newest)
* Published Date (Oldest)

### Historic updates ordering

* Relevance (default)
* Updated Date (Newest)
* Updated Date (Oldest)

> **Tip**: Selecting **Relevance** restores the default ranking calculated by the search engine.

## Advanced search syntax

There is a selection of operators and syntax available to perform advanced searches from the Global Search bar. Some that are commonly used include:

### Boolean operators: AND (+), OR, NOT (-)

* Must be in ALL CAPS
* OR is the default
* AND matches posts and comments that contain both words
* NOT excludes posts and comments that contain that word

### Wildcard searches: *, ?

* An * is used for a multiple character wildcard search
* A ? is used for a single character wildcard search
* Wildcards cannot be used at the beginning of a search term

### String search with quotations

* Placing two or more words within "double quotes" will search for that exact string.

## Request visibility

Some search results may be displayed but cannot be opened because of the Service Manager visibility model.

A request can be opened when one or more of the following conditions are true:

* You are the request owner.
* You belong to the team assigned to the request.
* You belong to a team that supports the request's service.
* You are a member of the request.
* You are the customer of the request.
* You raised the request.

If none of these conditions are met, the request reference is displayed but cannot be opened.

## Quick search

You can also use the quick search tool to find a specific request from any page in Hornbill. This is helpful when you have a reference ID and need to access a request immediately, such as during a phone call with a customer or a colleague.

![Quick Search for Requests](/_books/servicemanager-user-guide/images/request-quick-search.png)

### Steps

1. Press **Ctrl+Shift+F** on your keyboard. The quick search window opens.
2. Type the full or partial **reference ID** into the search field.
3. Press **Enter**.

### Expected result

The request associated with that ID opens automatically.

### Search tips for partial IDs

If you do not know the full ID, you can enter a partial ID. This is useful if you are unsure of the prefix or the number of leading zeros.

* **Accuracy**: The search is more accurate when you enter more numbers.
* **Multiple matches**: If your search matches more than one request, Hornbill opens the most recently created request.
