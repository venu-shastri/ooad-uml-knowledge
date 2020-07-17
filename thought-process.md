# ThoughtProcess

- Passion
- Vision 
	- Build For Last
	- Build For Change
- Requirement Analysis
	- Functional and Non-Functional Requirements
		- Use Case Diagram - Functional Requirements
			- useCase , actors, association , boundary , relationships (include , exclude)
- Analysis of Structural Elements - Logical View
	- Paradigm
		- Object Orientation 
			- Concepts
				- Encapsulation
					- Define Role and Responsibilities
					- Principles - SRP
					- Avoid GOD Class Design
						- GOD -> Does Everything
					- Uml Representation - Class Diagram
					- Cohesion - High
				 - Re-usability
					 - Relationship
					 - Types re-usability
				   
| Code Reuse | Object reuse  |
|--|--|
| Inheritance | Association [Composition , Aggregation] |

####  Inheritance
 - is-a relationship
 - Complete Code Reuse
 - One role assumes another role
 -  Classification ( Generalization and Specialization )
 - Family of Classes ( Commonality and Variation)
 - ex:-  **`Car is-a Vehicle`** , **`Radar is-a Sensor`** , **`MPCVideo is-a Sensor`**
 - Inheritance Limitations
	 - Static Relationship  (Re-Compile)
	 - Multiple Inheritance  issues (Diamond Problem)
		 - redundancy
		 - Dilemma
	- Ripple  Effect
	
#### Object Reuse
- uses relationship (has-a)
- One Object uses Another Object
- ex:-  **`Cluster uses/holds GPS Sensors`** , **`Camera uses/Contains Imager`** , **`System uses/Contains Processors`** , **`Radar uses/contains Antenna`**
- Association 
	- Associated
	- Referential Attribute
- Composition
	- contains
	- Death Relationship
- Aggregation
	- holds
	- part-of
- Principal :- Dependency Inversion principle
	- Abstraction (Unnecessary Information Hiding)
	- Loosely Coupled Solution
	- Program For Interface not for implementation
- Advantages Uses Relationship
	- Dynamic 	Relationship
	- Lazy Instantiation
	- No Ripple Effect
	- Easy to alter Cardinality  (Number of instances participate in given relationship)
### Prefer Composition over Inheritance

### Abstraction
- Abstraction b/w objects
- Let Object depend on interface of another object, than implementation
- An object should know how to communicate / Contract
- use Runtime polymorphism / function pointer to abstract 
- steps
	- identify Low Level module and Extract interface 
	- Let High Level Module Depends on interface of Low Level Module

### interface
- public view of object
- contains/define/describe contract ( method signatures)
- c++ -class - pure virtual methods / struct with function pointers
- UML - Realization/Generalization Notation
- Interface cannot be instantiated
- Given Object Can implement/realizes multiple interface
- Design issues
	- Fat Interface ( unnecessary methods)
		- Decompose Fat interface in to required multiple interfaces  (Interface Segregation Principle)
		- ISP - no client (consumer / implementor) should be forced to depend on methods it does not use
- name convention :- let interface name begin with - "I-can-do" 



### Implementation View
- Component Based Architecture
- UML- Component Diagram
	- Implementation of System from Components perspective
	- StackHolder- developer
	- Describe Dependency b/w components
	- Required and Provided Interfaces


#### Process view
- Activtity Diagram
	- De
- Timing Diagram
- Communication Diagram
- StateDiagram

#### Deployment View
- Deployment Diagram


				

					
					
		 
		  
 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI5Nzc0NDM5OCwtNTQ5NDc2OTAxLDc4NT
AzNzkzOCwtMjA3NDQ4ODg5NywtNTM0ODU5NDMxLDEwMjU5OTAx
MjUsMTY4MDk0ODIwNywxMzYzNzM5OTgwLC0yMzA2NTQxXX0=
-->