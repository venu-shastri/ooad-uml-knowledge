# Interaction Diagrams 
Interaction diagrams are used to illustrate interactions of
parts within a system.

There are 3 types of Interaction diagrams in UML
- Sequence diagrams
- Communication diagrams
- Timing diagrams

# Sequence Diagram

* [What is a Sequence Diagram](#SequenceDiagram)
* [Sequence Diagram Notations](#Notations)
	

### SequenceDiagram

Sequence diagrams, commonly used by developers, model the interactions between objects in a single use case. They illustrate how the different parts of a system interact with each other to carry out a function, and the order in which the interactions occur when a particular use case is executed.

In simpler words, a sequence diagram shows different parts of a system work in a ‘sequence’ to get something done.
### Notations
A sequence diagram is structured in such a way that it represents a timeline which begins at the top and descends gradually to mark the sequence of interactions. Each object has a column and the messages exchanged between them are represented by arrows.

**A Quick Overview of the Various Parts of a Sequence Diagram**

**Lifeline Notation**
A sequence diagram is made up of several of these
lifeline notations
- They should be arranged horizontally across the top of
the diagram
- No two lifeline notations should overlap each other
- They represent the different objects that interact with
each other in the system
- A lifeline notation with an actor element symbol is used
when the sequence diagram is owned by a use case

![Lifeline Notation](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/images/Sequence-diagram-Lifeline.png)

**Activation Bars**
> Activation bar is the box placed on the lifeline. It is used to indicate that an object is active (or instantiated) during an interaction between two objects. The length of the rectangle indicates the duration of the objects staying active.

> In a sequence diagram, an interaction between two objects occurs when one object sends a message to another. The use of the activation bar on the lifelines of the Message Caller (the object that sends the message) and the Message Receiver (the object that receives the message) indicates that both are active/is instantiated during the exchange of the message
![Activation Bar ](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/images/ActivationBar.JPG)

**Message Arrows**
- An arrow from the Message Caller to the Message Receiver
specifies a message
- The message can flow in any direction; from left to right, right to left and back to the caller itself
- The description of the message should go on the arrow
- Arrow heads may change according to different message types
- The message arrow comes with a description, which is known as a message signature, on it. The format for this message signature is below. 
**_message_name (arguments): return_type**

#### Different message types;
- Synchronous message
	- A synchronous message is used when the sender waits for the receiver to process the message and return before carrying on with another message
- Asynchronous message
	- An asynchronous message is used when the message caller does not wait for the receiver to process the message and return before sending other messages to other objects within the system
-  Return message
	- A return message is used to indicate that the message receiver is done processing the message and is returning control over to the message caller
- Participant creation message
	- objects can be created in the middle of a sequence. The dropped participant box notation is used when you need to show that the particular participant did not exist until the create call was sent.
-  Participant destruction message
	- participants, when no longer needed, can also be deleted from a sequence diagram. This is done by adding an ‘X’ at the end of the lifeline of the said participant
- Reflexive message
	- When an object sends a message to itself, it is called a reflexive message.

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5NTI2Njg2OCwtMTc0NTA0MTA1NCwtMT
gzNjA0MTYwNiwtMTYyNzEwMzM4NiwxNjA5NDEwMjkzLDE0MjM1
MjMwNTksMTgxODY2MzE2LDExMzY2NDc0Nl19
-->