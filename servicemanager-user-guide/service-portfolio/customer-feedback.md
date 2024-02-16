# Customer Feedback
To improve on the service you provide to your customers it is important to gather feedback from your customers on the level of service they have experienced when interacting with your teams. This feedback will enable you to highlight where exceptional services are being provided (and reward it), as well as highlight areas in which service could be improved and also if a consistent level of service is being provided overtime.

With the customer feedback feature, you can invite your customers to provide feedback on their requests once the requests are in a closed status.
* Feedback can be requested and provided through the customer and or service portals.
* You can include a link in your closure email templates directing customers to where the feedback can be provided.
* Feedback can be requested in the form of a simple star rating and or configurable feedback questions.
* Feedback can be enabled per request type (Incidents and Services Requests) and per service where it is required.
* Feedback requests can be open ended, or time limited.
* Feedback information can be viewed on the related request and or reported against using the reports building and advanced analytics in the admin tool.

## Enabling Customer Feedback
In each service record, under Request Configuration there is an option to enable Customer Feedback against each request type.
* By Default the Enable Star Rating will be enabled.
* By Default the Enable Questions will be disabled.

When configuring the customer feedback options, it is important to remember that you are only enabling or disabling the options for the specific request type, and against the specific service. Changes configured here are not global and will not impact other request types on the same service or other services you offer.

* **Enable Star Rating**<br>With this set to enabled, the customer will simply be able to provide a 1-5 star rating to feedback on the service they have received.
* **Enable Questions**<br>With this enabled any questions which have been configured will be presented to the customer when they are providing feedback. If you do not wish to show configured questions to the customer, simply disable this option you do not need to remove the questions themselves.
* **Feedback Expiry**<br>If required you can define the number of days the customer has to provide the feedback. If the value is set to 0, the request for feedback will NOT expire. If a number of days are selected, the request for feedback on a request will automatically be removed once the specified number of days has passed.

## Creating Customer Feedback Questions
If desired you can configure up to 5 feedback questions.

To add a new Question, simply select the Add Question button and complete the configuration options.

* **Question**<br>As it will appear to the customer on the customer or service portal.
* **Type**<br>Choose how the answer can be provided - Single or Multiline Text, Dropdown Box, Checkbox or Option Group, or a Button list.
* **Mandatory**<br>Choose if the customer is required to provide an answer to this specific question before they can submit their feedback.

If you have chosen a type which requires options such as a Button List, it is at this point you will be able to define the available options which will be presented to your customers.

* **Language**<br>By default the question will be created in the default language of your instance, if you wish to provide the question in different languages for your customers, simply choose the Add Translation button and choose the additional language or languages you wish to provide the question in, and define the question and options in those languages.
The same technique can be used to offer the available answers in different languages, by configuring each answer in the languages you require.

The customer's language will automatically be picked up from their profile, and the questions presented to them in the correct language (if this has been configured, alternatively they will be presented in the default language for your instance).

* You can easily choose to reorder how the questions are presented to the customer on the Customer or Service Portals, by simply picking up and dragging and dropping the questions into the desired order on the list of questions.
* You can change the maximum number of questions which can be defined via the the admin tool. Under Service Manager > Settings and the app.request.customerFeedback.maxQuestion setting.

## Providing Feedback
On both the Customer and Service Portals, customer will see a new Awaiting Feedback option on their request lists, when one or more of their closed requests is awaiting feedback. There is also a Drop Down option on their request list views to move between Active, Closed and Awaiting Feedback requests.

On opening a request which is awaiting feedback, the customer will be presented with the Customer Feedback pop up, presenting the options to complete the star rating and or any feedback questions which have been configured. The customer has three choices at this point:

* **Submit**<br>They can complete all or any mandatory questions and submit their feedback.
* **Later**<br> They can choose not to submit feedback at this time, and simply close the pop up - this feedback will then be presented again when they revisit the request.
* **No Thanks**<br>They can choose not to provide any feedback, and the pop up will disappear and they won't be prompted again on this request for feedback.

## Viewing Feedback
If a customer chooses to provide feedback, their feedback will be available on the request for them, and the owner or anyone else who has rights to view the request to see. A Collapsible panel will appear under the main details of the request, which will contain both the questions and the customers answers.