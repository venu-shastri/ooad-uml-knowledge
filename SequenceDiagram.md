# Interaction Diagrams 
Interaction diagrams are used to illustrate interactions of
parts within a system.

There are 3 types of Interaction diagrams in UML
- Sequence diagrams
- Communication diagrams
- Timing diagrams

# Sequence Diagram

* [What is a Sequence Diagram](#Sequence-Diagram)
* [Sequence Diagram Notations](#Notations)
* [Sequence Fragments](#Sequence-Fragments)
	

### Sequence-Diagram

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

![Message Types](https://raw.githubusercontent.com/venu-shastri/ooad-uml-knowledge/master/images/Sequence-diagram-MessageTypes.png)

### Sequence-Fragments
- Sequence fragments are used to show complex interactions such as alternative flows and loops in a more structured way.
- A sequence diagram is drawn as a box that frames a section of nteractions between objects in a sequence diagrams.
- On the top left corner of the fragment sits an operator. This – the fragment operator - specifies what sort of a fragment it is.
- Fragment Types
	- Alternative Combination Fragment
	- Option Combination Fragment
	- Loop Fragment
	- Reference Fragment
#### Alternative-Combination-Fragment
- It is used when a choice needs to be made between two or more message sequences. 
- It models the **“if then else”** logic
-  It is specified by mentioning **‘alt’** inside the frame’s name box
- To show 2 or more alternatives, the frame is divided into what is called **interaction operands** using a dashed line
- Each operand has a **guard** to test against and it is placed at the top left corner of the operand

![Alternative](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/images/Alternative-fragment-example-1.png)

#### Option Combination Fragment
> The option fragment is used to indicate a sequence that will only occur under a certain condition, otherwise the sequence won’t occur
• It models the **“if then”** statement
• It is represented with a rectangular frame where **‘opt’** is placed inside the name box
• Unlike the alternative fragment, the option fragment is **not divided to operands**

![Option](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/images/Example-of-an-option-fragment.png)

#### Loop Fragment
>It is used to show a **`repetitive sequence`**
• It is drawn as a frame and specified by placing **`loop`** in the name box
• It can be used
– for the Boolean test
– to test minimum iterations (the loop must execute not less than the number mentioned)
– to test maximum iterations (the loop mustn’t execute more than the number mentioned)

![Loop](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/images/New-Loops-Sequence-Diagram-Example-1.png)

#### Reference Fragment
>It allows you to reuse or refer to a part of one sequence diagram in another
• It helps **`manage the size of large sequence diagrams`**
• Include **`ref`** in the name box of the frame to specify the reference fragment
• Mention the name of the sequence diagram being referred to inside the frame
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTU1NTgwNDk1OSw5Mjk0OTY5MDAsMTE2Mj
A3MDY5MCwtODI0NDg4MDksLTEzOTIyNDcyOTcsLTE3NDUwNDEw
NTQsLTE4MzYwNDE2MDYsLTE2MjcxMDMzODYsMTYwOTQxMDI5My
wxNDIzNTIzMDU5LDE4MTg2NjMxNiwxMTM2NjQ3NDZdfQ==
-->