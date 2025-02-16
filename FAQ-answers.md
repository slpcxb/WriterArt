
1. How can I send a single “Hello World” message to myself?

A: You can use the `subscribers` parameter and specify your own phone number as the value of the parameter.

2. What are my options for selecting which of my subscribers receive a message I send via the API?

A: You have the following options:
* Use `subscriberIds` to specify a list of subscriber ids.
* Use `subscribers` to specify a list of phone numbers or email addresses of the subscribers.
* Use `allSubscribers` to make the system send the message to all subscribers.
* Use `groups` to specify a list of group ids.

3. What information is available in response to an API call to send a message?

A: The response contains the following information:
* The message Id.
* The total number of messages sent by this API call.
* The total number of failed messages sent to international recipients.
    
4. How do I schedule a message to be sent in the future?

A: You can use the `scheduledDate` parameter and specify a future date.
    
5. Can I refer to my subscribers by name in the message I send to them?

A: By inserting a `firstName` Liquid Template variable into your message and using the `properties` field that include the `firstName` property, you can refer to subscribers by name.