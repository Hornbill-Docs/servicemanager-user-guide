# Solutions action

The Solutions action helps you identify and apply fixes to an incident. The **Solutions** icon is dynamic. It only appears in the interface when the system finds a potential solution for that specific incident.

If an incident links to one or more problem or known error records that contain defined workarounds, the system displays these workarounds as possible solutions.

## Before you begin

An administrator must enable the solutions action within the [Request Configuration](/servicemanager-user-guide/service-portfolio/request-configuration#request-actions) for each service.

## Use a solution

When a linked known error or problem record contains a workaround, you can review it in the **Solutions** tab.

To manage these solutions, follow these steps:

1. Open the incident and select the **Solutions** action.
2. Review the list of available solutions.
3. Select an action from the drop-down menu for a specific solution:
    * **Accepting a solution**: Select this to mark the solution as accepted. The solution turns green and displays as an **Accepted Solution**. The system automatically copies the solution text into the **Resolution** text box.
    * **Not the solution**: Select this if the solution does not resolve the incident. The record then displays as **Not the Solution**.
4. If you accept a solution, the incident is ready for the incident owner to resolve using the copied text.

<!-- [Visual Cue: Annotated screenshot showing the Solutions icon in the request action bar and the color change when a solution is accepted.] -->

## Use FAQs as solutions

If an FAQ is published against the same service as the request and has visibility set to **Service Desk**, it appears under the **FAQ** tab of the **Solutions** action.

You can interact with FAQs in the same way as standard solutions:

* **Accepting a solution**: Select this to highlight the FAQ in green. The text copies to the **Resolution** text box.
* **Not the solution**: Select this to mark the FAQ as incorrect for this incident.
* **Resolve using a solution**: Once you accept an FAQ, the text is ready in the **Resolution** box for the incident owner to complete the resolution.

## Access knowledge articles

Knowledge articles appear in the **Solutions** action if they belong to a knowledge base linked to the same service as the request.

* You can use the provided filter to find specific articles. This filter searches the titles of the articles only.
* [Knowledge base subscriptions](/servicemanager-user-guide/knowledge/knowledge-bases/subscriptions#service) provide access based on the related service of the request.

<!-- [Visual Cue: Diagram showing the relationship between Services, Knowledge Bases, and the Solutions action.] -->
