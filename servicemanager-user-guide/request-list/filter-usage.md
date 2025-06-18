---
layout: article-toc
---
# Optimizing filter usage in views
 
The Filter box, highlighted in red below, is often misunderstood, leading to missed results or performance problems. Its purpose is to narrow down your existing view by searching for whatever you enter across several predefined fields. These fields include: 

* Summary 
* Description 
* Hornbill Reference 
* External Reference 
* Customer Name 
* Priority 
* Organization Name 

![Quick filter and Advanced search in views](/_books/servicemanager-user-guide/request-list/images/quick-filter-advanced-filter.png)

This filter performs a *double wildcard* search. This means it looks for the text you enter *anywhere* within the fields listed above. While this might seem convenient, it's actually **extremely inefficient** and can frequently return inaccurate results. In fact, it's the primary cause of performance slowdowns and why you might sometimes get no results at all. Although this functionality still exists, its use is strongly discouraged and may be removed or changed in future updates. 

For accurate and efficient searches, you should **always use the advanced search fields**, highlighted in green. These fields allow you to target specific criteria, ensuring your search is precise and performs optimally. By using Advanced search, you can directly specify the field you want to match, which is much more effective than the broad, inefficient Filter function.

To access the advanced search fields, click **Advanced** to the right of the Filter box.

![Advanced search in views](/_books/servicemanager-user-guide/request-list/images/advanced-search.png)

Another option, which you might find to be even faster, is to search on Requests using the global search field in the Hornbill toolbar. Click the down arrow in the search field before entering your search term to access the filters shown below.

![Quick filter and Advanced filter in views](/_books/servicemanager-user-guide/request-list/images/main-search-on-requests.png)

## Common issues
We often hear about performance hiccups with the My Requests view, and usually, they boil down to one of three common issues.

### No limiting criteria
One of the biggest culprits for slow performance is not setting any limits on your view. The filters in My Requests are dynamic, meaning they adjust based on the selections made by the agent who created them. If not properly configured, this can result in the system trying to pull incredibly large and inefficient datasets --- sometimes every single call ever logged
since day one!

**The fix:** Take a moment to think about exactly what you want to see. Even a small change, such as adding a filter where *Date Last Modified* is greater than the *Start of this year*, can drastically improve performance by narrowing down the data the system must process.

### Too much limiting criteria
On the flip side, sometimes users go overboard with their filters, ironically making the view useless. Adding every single team individually, or including every call status, or listing all service IDs one by one, essentially defeats the purpose of filtering. It's crucial to remember
that the My Requests list filters aren't meant to replace comprehensive reports.

**The fix:** Simplify your filters. For instance, if you're trying to view too many call statuses in one go, reduce that number. It's far more efficient to create separate views for each call status you want to track. This not only improves performance, but also makes your views much clearer and more focused.

### Outdated historic filters
It's common for views to be created and then never updated. Over time, these static views might no longer follow best practices or take advantage of new features that could significantly improve their efficiency.

**The fix:** Regularly review your existing views to ensure they're still efficient and up to date. A classic example of an outdated filter is a hardcoded date field, such as *Log date is greater than 2022*, when we're now well past the year 2022. These static dates need to be adjusted or replaced with dynamic options to keep your views relevant and performant.

## Addressing performance issues in your Request List
We understand that a slow Request List can be frustrating, and Hornbill is committed to ensuring a smooth experience for all users. When we identify significant performance issues within your instance's Request List, we'll reach out directly to your designated primary and secondary contacts. We'll ask them to collaborate with the affected end users to implement the solutions we've discussed, such as refining search criteria and
updating old filters.

## Your feedback matters!
We're always looking for ways to improve your experience. We'd love to hear any feedback you have on how we can make searching for requests a more efficient and pleasant task. Your insights are invaluable in helping us enhance the system for everyone.

## Hornbill's right to implement limits
In the rare circumstance that, despite our escalations, changes aren't made to existing customer instance views causing persistent performance degradation, Hornbill reserves the right to add limits to request views. This is a measure we hope to avoid, but it's essential to maintain the stability and performance of the platform for all users.