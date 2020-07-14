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


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEwOTI0ODU2MDUsLTE2MjcxMDMzODYsMT
YwOTQxMDI5MywxNDIzNTIzMDU5LDE4MTg2NjMxNiwxMTM2NjQ3
NDZdfQ==
-->