# Notification System Design #

Notification is one of most usable feature in each and every app available in the internet.

Functional req. 
	1. Ability to send and receive notification.
	2. Pluggable: easy to add new features
	3. Saas: Rate limit on number of notification to send on multiple products
	4. Prisonization : Some messages need low priority eg likes and comments but some needs high priority eg OTP, payment related messages.

Non Functional req.
	1. High availability
	2. Scalable.

To build this we need to take care so many things
	1. We don’t need to build queues like process to send message either we can use kafka or AWS SQS  or Azure Service Bus
	2. Then some component needs to work and make sure its working correctly eg. MessageValidatior, Prisonization tools etc
	3. What type of message client want to receive SMS, Email or customer made notification component
	4. According to situation we need to decide message queue will synchronous or asynchronous.
Handlers
	1. Email Handler
	2. In-App Handler
	3. IVRS Handler: For High value orders, send a IVRS cal
	4. Notification Tracker
	5. Bulk Notification
	6. Query Engine
	7. Scheduler
	8. Pipelines
	9. Batch jobs
