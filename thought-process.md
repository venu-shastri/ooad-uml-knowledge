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

### Abstraction
- Abstraction b/w objects
- Let Object depend on interface of another object, than implementation
- An object should know how to communicate / Contract
- use Runtime polymorphism /  to abstract 
				

					
					
		 
		  
 
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTk1OTA0MTQ5MywxMDI1OTkwMTI1LDE2OD
A5NDgyMDcsMTM2MzczOTk4MCwtMjMwNjU0MV19
-->