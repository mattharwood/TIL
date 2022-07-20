# Define a message or event when the contract isn't yours

In NServiceBus, you may want to send a message, event, command etc. that your code is a client of, and it does not impliment an NServiceBus interface (such as IEvent, IMessage).

To overcome this, you can define what constitutes an event or message through "Conventions". On your endpoint configuration, add:

===================================================================
var conventions = endpointConfiguration.Conventions();
conventions.DefiningEventsAs(type => type.Name.EndsWith("Event"));
===================================================================