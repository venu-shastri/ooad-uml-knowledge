# Logical View (Object Oriented Decomposition)
>This view focuses on realizing an application’s functionality in terms of structural key elements, key abstractions and mechanisms, separation of concerns and distribution of responsibilities.
>- Vertical and horizontal divisions The application can be vertically divided into significant functional areas (i.e., order capture subsystems, order processing subsystems).
>Or, it can be horizontally divided into a layered architecture distributing responsibilities among these layers (i.e., presentation layers, services layers, business logic layers, and data access layers).

>- Representation of structural elements as classes or objects and their relationships.

## Design Concepts
- Object

- Roles

- Responsibilities and Collaborations

- Relationships

- Principles

- Patterns

### Designing  the application using several complementary perspectives
- An Application
	- Set of interacting Objects
- An Obejct
	- An Implementation of One or More Roles
- A Role
	- A Set of Related Responsibilities
- A Responsibility
	-  an obligation to perform a task or know information
- A Collaboration
	- an interaction of objects or roles (or both)
- A Contract
	- an agreement outlining the terms of a collaboration

### Object design
![Object Machinary](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/images/Object_machinary.JPG)


- Define its Public Interface

- The terms and Conditions of  Use

- The Private Details – how it conduct its bussiness



>"The object has three properties, which makes it a simple, yet powerful model building block. It has state so it can model memory. It has behavior, so that it can model dynamic processes. And it is encapsulated, so that it can hide complexity."
Trygve  Reenskaug

#### Object Role Stereotypes
- information holder—knows and provides information

- Structurer—maintains relationships between objects and information about those relationships

- Service provider—performs work and, in general, offers computing services

- Coordinator—reacts to events by delegating tasks to others

- Controller—makes decisions and closely directs others' actions

- Interfacer—transforms information and requests between distinct parts of our system
#### Responsibilities?
>Object Responsibilities include three major items:

- The actions an object performs

- The knowledge an object maintains

- Major decisions an object makes that affect others

>Do not try to design objects to have all the conceivable behavior shown in the real world. Rather, make software objects only as smart as the application needs them to be and no smarter
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTA3MTYxMzI5MywtMjA1NzMwOTMyN119
-->