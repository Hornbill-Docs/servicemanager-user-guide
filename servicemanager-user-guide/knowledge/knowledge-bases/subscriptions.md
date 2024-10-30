# Subscriptions
The purpose of Subscriptions is to manage who can access a knowledge base.  The subscription access focuses on the readers. The starting point for all knowledge bases is that they are accessible to all users that have the Knowledge User role. You only need to add subscriptions if there is a need to restrict access.

## Subscription Types
### Service
With an established implementation of Service Manager, it is likely that the services you provide are already defined.  Each service can have its own subscription list where access is limited to those who need to consume that service.  

The `Service` type in the Knowledge Base Subscriptions takes advantage of the existing Service Subscriptions.  This is particularly useful when you want to create a knowledge base that supports one or more services.

Users with the Knowledge Base Manager role can control knowledge base access through service subscriptions. For example, a service called Desktop Support can be given a subscription to a knowledge base called Hardware Troubleshooting. All end users who have the Desktop Support service will then have visibility of the Troubleshooting knowledge base.

### Team
Teams in Service Manager are restricted to full users who are subscribed to Hornbill. The `Team` type in the Knowledge Base Subscriptions will provide access to all the members of the team.  Using Teams is ideal for when you have a knowledge base that supports your support teams.  This type of knowledge base might contain technical articles that wouldn't be suitable for user consumption.  

## Adding Subscriptions
**To add a subscription to a knowledge base:**
1. Navigate to **Service Management** > **Knowledge** > **Knowledge Bases**.
1. In the list of knowledge bases, click the Name link for the knowledge base to which you want to subscribe a service.
1. In the Knowledge Base navigation pane, click **Subscriptions**.
1. Click the plus button, then in the Service field, begin typing the name of the service you want to give a subscription to.
1. From the dropdown, select the service and click **Add**.

**To view subscriptions by knowledge base:**
1. Navigate to **Service Management** > **Knowledge** > **Knowledge Bases**.
1. In the list of knowledge bases, click the Name link for the knowledge base you want to check.
1. In the Knowledge Base navigation pane, click **Subscriptions**.

    Any subscribed services will be displayed in a list.

**To view knowledge-base subscriptions by service:**
1. Navigate to **Service Management** > **Service Portfolio**.
1. In the list of services, select a service.
1. Click the Knowledge Bases button (the book spines).

    Any knowledge-base subscriptions attached to service will be displayed in a list. You can go straight to the subscribed knowledge base by clicking the eye icon.