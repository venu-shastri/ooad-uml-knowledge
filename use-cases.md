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
## Use Case Building Blocks
- Subject
- Actors
- UseCase

###  Actor
- Include all user roles that interact with the system
- Include system components only if they responsible for initiating/triggering a use case.
	- For example, a timer that triggers sending of an e-mail reminder
- An actor represents a set of roles that users
of use case play when interacting with
these use cases.
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
### What is a user story?
- An abbreviated description of a use case
- Used in agile development
- Answers 3 questions:
	- Who?
	- Does what?
	- And why?
> As a  **type of user** , I want **some behavior from the system** so that **some value is achieved**
![User story](https://github.com/venu-shastri/ooad-uml-knowledge/blob/master/UseStory.JPG)




<!--stackedit_data:
eyJoaXN0b3J5IjpbMTU1Mzc4MDY5OSwyMTQxNzQxNzIwLDMxMD
AwMjUwNF19
-->