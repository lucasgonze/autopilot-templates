SMS Listserv
============

A user-friendly alternative to SMS-based chat groups, based on Twilio Autopilot

An SMS-based chat group is ordinarily created by having one person send a text to a set of recipients, rather than just one. When these groups take on a life of their own rather than disappearing quickly, they have weak user experience. 

For example, I am one of 13 people in an SMS group for my son's soccer team. Every week I get 5-10 texts. One mom wanted to add her husband but couldn't. Half of the messages I see only have a number, and not a name. Several kids left the team but their parents can't leave the group.

This project will use the Twilio API to improve on SMS groups:

1. A participant will be able to remove themself from the thread. Ordinarily that is impossible after the thread starts.
2. A participant will be able to add themself to the thread. Ordinarily that is impossible once the thread has gotten started.
3. A participant will be able to set their name and other metadata, like email address. Ordinarily every participant needs to have every other participant in their address book in order to see their name, and participants have no way to find names for numbers not in their address book.
4. A sender will only have to send to a single number, not to a collection.
5. A recipient will receive from a single number, and will be able to block or filter that number. Ordinarily chats come from a combination of all the numbers and are nearly impossible to filter.

To create a new SMS group: 
1. Start normal group chat by adding number after number after number
2. Add the number of the service to the participants
3. Send the first message, press enter 
4. The chatbot will send a message out to the whole group to start a new thread

Note that there would then be two threads. This problem could be neutralized if the chat-based UX was supplemented by a mobile app. The mobile app would intercept outgoing group SMS chats and replace them with sms-listserv chats. 

The mobile app could also enhance participation by adding GUI affordances. GUI features:

* removal from a thread, even if not created via sms-listserv
* addition of metadata like name and email address

UX of the bot will be modeled on Mailman. Commands will be based on email listservs:

* help: a list of available commands will be sent
* subscribe <phone number>: add a person to the group
* unsubscribe: leave the group
* quit: leave the group
* remove me: leave the group
* who: get a list of group members
* info: learn who created the list



This is a concept app for the moment. There is no code yet.

