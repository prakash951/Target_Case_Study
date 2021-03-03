# Target_Case_Study
Target Case Study On Event Sourcing

Generic Notification System 
 
Problem Statement 
Most applications have the need to implement notifications for a variety of use cases and
scenarios. Create a centralized generic service for notification that can be used by a variety
consuming application for their notification needs e.g. an incident workflow system may use
this system when each incident ticket moves from one state to another, similarly a order
management system may use this service to notify the customer of the status of the order
whenever it changes 
 
The system should allow for the following capabilities: 
 
1. Accept messages including from, to and subject 
2. Ability to notify on multiple channels (e.g email, slack, you can stub out/mock if
required) 
3. Deliver messages in correct order for each consumer of this


Approach:

Using a Messaging system such as kafka or rabbitmq to register the event, there would be multiple subscribers who are listening to specific topic, those consumers are notified with the event and cosumers will take appropriate action based on the event. 

The following demo will show how event sourcing will be used notify the slack and e-mail consumers.

Tech Stack Used:

Apache Kafka
Slack
Spring Boot
JDK 11

Steps to follow to configure the notification system with 2 consumers

1). Create a kafka topic
    ![image](https://user-images.githubusercontent.com/6679672/109767744-02a28300-7c1e-11eb-8511-1f84b46e2300.png)
    
2). Create a slack channel
    ![image](https://user-images.githubusercontent.com/6679672/109767910-3aa9c600-7c1e-11eb-9a53-496607e950b1.png)









