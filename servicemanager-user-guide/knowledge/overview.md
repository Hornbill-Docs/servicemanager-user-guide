---
layout: article-toc
---
# Overview
Knowledge within Service Manager is an invaluable resource for organizing, storing, and sharing your organization's information. With Knowledge, your organization's collective expertise can be developed collaboratively and easily shared --- internally and externally. Use Knowledge to gather your staff's insights, know-how, and resolutions all in one place for everyone's use.

**Self-service.** Built for agent deflection and self-service, Knowledge is fully integrated into the self-service experience, as well as the Intelligent Capture logging experience for analysts. Everything your organization puts into your knowledge bases can be searched across the entire Hornbill platform using global search, with customizable gating in place to ensure Knowledge consumers see only the content meant for them. For more details on how end users can view the content of your knowledge bases, see [Search/Browse](/search-and-browse).

**Subscriptions.** Hornbill Service Manager provides a join between knowledge bases and services; you can set up [a subscription model](/knowledge-bases/subscriptions) to meet your organization's specific needs based on the Knowledge content you have and the services you offer. When you first create a knowledge base, by default it's open to all. To restrict access, you add knowledge-base subscriptions to individual services. Users who can see an individual service can then see the knowledge bases that service subscribes to.

**Access.** [Roles](/servicemanager-config/setup/service-manager-roles#knowledge-roles) determine who can do what to knowledge bases. Those with the Knowledge Manager role can further customize who can create content by controlling [*contributor access*](/knowledge-bases/contributor-access). Knowledge Base Managers can grant access for content creation to named teams or users. This access is independent of service subscriptions; for example, you could add the Finance department to your knowledge base to allow the staff of that department to contribute content and edits.

**Approvals.** Hornbill Knowledge provides publishing and auditing processes for [ensuring quality and review stages](/knowledge-bases/activity-and-audit).

**Analytics.** Hornbill Knowledge captures metrics such as article views and likes that you can view in [customizable charts](/dashboard), along with [search data](/search-data). By tracking usage and effectiveness, you can identify gaps and continually improve content and accessibility.

## Why does knowledge matter?
* When information is not easily accessible within an organization, it can be time-consuming and costly for staff to have to rediscover how something was configured, how a previous issue was resolved, or how something works. Having an organization's shared knowledge stored and readily accessible frees staff to work on meaningful tasks.
* A well-implemented knowledge system allows all the experts in an organization to easily contribute. Capturing and sharing information is key to the efficiency of those who are on both sides of the service desk.
* By enabling efficient access to relevant information, reducing redundant efforts, and promoting self-service, Hornbill Knowledge can drive significant operational efficiencies for your organization. Use Knowledge to streamline incident resolution, improve service quality, and reduce costs, all while enhancing the overall productivity of both your staff and your service end-users.

## Before you begin
* Review the available [knowledge roles](/servicemanager-config/setup/service-manager-roles#knowledge-roles) that can be assigned to the different types of users.
* Consider the [types of articles](/servicemanager-config/knowledge/article-types) that you will want to provide in your knowledge bases.
* Consider the audiences you want your knowledge bases to serve.
* Consider the roles you might assign for contributing and viewing content.

## About the Knowledge structure
At the top level of Knowledge is the knowledge base. Inside the knowledge base are *topics*, which you can think of as folders and sub-folders that contain articles.
* **Knowledge bases.** You may want to build out only one knowledge base, or you may want several. There is no limit to how many knowledge bases your organization can have.
* **Topics.** You can use [topics](/servicemanager-user-guide/knowledge/knowledge-bases/topic-structure) to provide a hierarchical structure that is unique to each knowledge base. Topics are not required, but when you do choose to use them, they provide an easy-to-navigate tree that contains Knowledge articles. Topics can be moved around in the structure of a knowledge base, and they can go up to five levels deep.
* **Articles.** Individual [articles](/servicemanager-user-guide/knowledge/knowledge-bases/articles) that contain your Knowledge content.

![Knowledge Structure](_books/servicemanager-user-guide/knowledge/images/knowledge-structure.png)

## Creating knowledge
Your organization can build knowledge bases in many ways:

* Reuse content from the resolution of incidents.
* Migrate your Service Manager [FAQs](/knowledge-bases/articles#moving-faqs-into-knowledge-bases).
* Capture staff know-how by granting [contributor access](/knowledge-bases/contributor-access).
* Create articles from requests.
* Create articles based on research.
* Use HAi for [automatic creation of articles](/hai/knowledge-generator).

## Sharing knowledge
Using Hornbill Knowledge to share your organization's collective expertise, you can:
* Suggest knowledge to end users during the raising of a request.
* Assign support staff to help find solutions.
* Promote popular articles via portal widgets.
* Allow users to search Hornbill Knowledge globally within Hornbill as well as externally.
* Provide the browsing of knowledge bases and their topics.