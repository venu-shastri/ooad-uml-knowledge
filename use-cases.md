# Use case
- Requirements analysis concept
- Describes the system's actions from a the point of view of a user
- **Tells a story**
	- A sequence of events involving
	- Interactions of a user with the system
- Specifies one aspect of the behavior of a system, **without specifying the structure of the system**
- Is oriented toward satisfying a user's goal

## How do we describe use cases?
- Textual or tabular description
- User stories
- Diagrams
### What is a user story?
- An abbreviated description of a use case
- Used in agile development
- Answers 3 questions:
	- Who?
	- Does what?
	- And why?
> As a  **type of user** , I want **some behavior from the system** so that **some value is achieved**
![User story](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/UseStory.JPG)


### Use Case Diagrams
- A picture
- describes how actors relate to use cases
and use cases relate to one another
- Diagrams are not essential
- They are helpful in giving an overview, but only secondary in importance to the textual description
- They do not capture the full information of the actual use cases
- In contrast, **text** is essential
- Objectives
	- Built in early stages of development
	- Purpose
		- Specify the context of a system
		- Capture the requirements of a system
		- Validate a systems architecture
		- Drive implementation and generate test cases
		- Developed by analysts and domain experts
### How do use case diagrams fit in?
![usecasefit](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/usecase-fit-in.JPG)

Diagram reproduced from www.edrawsoft.com.

![UsecaseDiagram](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/UseCaseDiagram.JPG)

## Elements Of UseCase Diagram
- Subject
- Actors
- UseCase

###  Actor

![Actor](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/Actor.JPG)
-Actor is someone interacting with use case (system function). Named by noun.
- Similar to the concept of user, but a user can play different roles; (example: a prof. can be instructor and researcher – plays 2 roles with two systems).
-  Actor triggers use case.
- Actor has responsibility toward the system (inputs), and Actor have expectations from the system (outputs) 
- Include all user roles that interact with the system
- Include system components only if they responsible for initiating/triggering a use case.
	- For example, a timer that triggers sending of an e-mail reminder.
- Actors can be human or automated systems.
#### Finding Actors
##### External objects that produce/consume data:
- Must serve as sources and destinations for data
- Must be external to the system

![actor](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/actors.JPG)

##### Questions to find actors
- Who are the system’s primary users?
- Who requires system support for daily tasks?
- What hardware does the system handle?
-  Which other (if any) systems interact with the system in question?
- Do any entities interacting with the system perform multiple roles as actors?
- Which other entities (human or otherwise) might have an interest in the system's output?

### Use Case
![usecase](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/usecase.JPG)
- System function (process – automated or manual).
- Named by verb.
- Each Actor must be linked to a use case, while some use cases may not be linked to actors.

### Elements of use case diagram: **Other details**

![others](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/usecaseotherelements.JPG)

### Linking Use Cases
- **Association** relationships
- **Generalization** relationships
	- One element (child) "is based on" another element (parent)
- **Include** relationships
	- One use case (base) includes the functionality of another (inclusion case)
	- Supports re-use of functionality
- **Extend** relationships
	- One use case (extension) extends the behavior of another (base)

#### Association
>Relationships between Use Cases and Actors
>Actors may be connected to use cases by associations, indicating that the actor and the use case communicate with one another using messages.

![Association](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/Association.png)

#### Generalization
- The child use case inherits the behavior and meaning of the
parent use case.
- The child may add to or override the behavior of its parent.
![Generalization](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/Generalization.png)

#### include
- The base use case explicitly incorporates the behavior of another use case at a location specified in the base.
- The included use case never stands alone. It only occurs as a part of some larger base that includes it.
- Enables us to avoid describing the same flow of events several times by putting the common behavior in a use case of its own.
- Include relationship – a standard case linked to a mandatory use case.
- Example: to Authorize Car Loan (standard use case), a clerk must run Check Client’s Credit History (include use case).
- The standard UC includes the mandatory UC (use the verb to figure direction arrow).
- Standard use case can NOT execute without the include case **tight coupling** .

#### Extend
- The base use case implicitly incorporates the behavior of another use case at certain points called extension points.
- The base use case may stand alone, but under certain conditions its behavior may be extended by the behavior of another use case.
- Enables to model optional behavior or branching under conditions
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc1ODc2NTgwNyw3MzU4MTc5NCw5OTI3Mj
MzMzMsLTM3MTUxNjgzOSw2NzYyNzE4OTQsMTI4NzAyMTgyMiwt
NTEwMjg4NzcxLDIxNDE3NDE3MjAsMzEwMDAyNTA0XX0=
-->