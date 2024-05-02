# Global Search for Requests
The Global Search for Requests allows you to locate Service Manager requests, including incidents, problems, changes, and service requests. When using the Global Search a number of entities can be selected on the left hand side of the service. The Requests entity will only be available when Service Manager is installed and will only be visible to user that have rights to use Service Manager.

## Search Bar
The search is a natural language search where you can type in anything from a single word to a sentence into the Search Bar. The text typed into the search bar will search the following fields of a request

* Request ID
* Summary
* Description
* External Reference Number

## Search Tools
The Search Tools are accessed by an arrow located on the right-hand side of the search field. By clicking on this arrow the following search options are made available to improve your search.

* **Any Type**<br>Allows you to select a single request type to be included in the results page. The requests types include Incident, Service Request, Change, Problem, and Known Error.
* **Any Status**<br>Allows you to select a single status of requests to be included in the results page. The statuses include New, Open, Close, and Resolved
* **Any Owner**<br>A single owner can be selected using the Co-worker search. Once a co-worker is select, only the requests where that co-worker is the owner, will be in the results
* **Any Customer**<br>A single customer can be selected using the customer search. The Seach Customer will return both contacts and co-workers. Once a customer is selected, only requests where that contact or co-worker is the customer of the request will be displayed.
* **Any Service**<br>Select a single service from the list of services to produce search results that only contain requests belonging to that service
* **Details or Timeline**<br>When searching you can select if you want to search the details of the requests or the Timelines. The Details search is the default search where the provided search string will match with information held in the Summary, Details, Owner, Customer, and Request ID. If Timeline is selected, the provided search string will be match information held in the Timeline of the requests.

:::tip
If a migration from the Supportworks application has included the importing of request records, the history on these records will be available on an ooption titled Historic Requests.
:::

## Advanced Search
There is a selection of operators and syntax available to perform advanced searches from the Global Search Bar. Some that are commonly used include:

### Boolean Operators: AND (+), OR, NOT (-).
* Must be in ALL CAPS
* OR is the default
* AND matches posts and comments that contain both words
* NOT excludes posts and comments that contain that word

### Wildcard Searches: *, ?
* An * is used for a multiple character wildcard search
* A ? is used for a single character wildcard search
* Wildcards cannot be used at the beginning of a search term

### String Search with Quotations
* Placing two or more words within "double quotes" will search for that exact string.

## Search Results
You may not be able to access some search results because of the Service Manager visibility model
When browsing your list of search results, you may notice that the link to some requests is inactive. This is due to the Service Manager visibility model. During a search, the application checks a number of criteria about the request to understand if you should be allowed to access it.

The visibility logic is as follows:
* Are you the owner of the Request?
* Are you a member of the team that the Request is assigned to?
* Are you a member of a team that supports the Service that the Request has been raised against?
* Are you a member of the Request?
* Are you the customer of the Request?
* Did you raise the Request?

If any of these are true, you will be able to click on the request summary and view it in its entirety.

## Quick Request Search
If you already know the Request ID you are looking for, you can use the quick request search option from anywhere in Hornbill.

Simply use Ctrl + Shift + F to open the quick search pop up where you can enter the request ID and open the request (if you have the appropriate rights to view the request).

<!-- https://wiki.hornbill.com/index.php?title=Global_Search_for_Requests -->