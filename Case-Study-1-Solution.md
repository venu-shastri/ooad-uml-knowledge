# Financial Risk Management System

## Functional Requirements

> - Import TradeData From TDS 
> - Import Counter Party Data From RDS
> - Co-Relate (Merge) Trade and Counter Party Data
> - Risk Calculation
> - Generate Risk Calculation Report
> - Export Risk Calculation report - Excel Format
> Configure Risk Calculation  - Risk Parameter

### Verbs
- import
- export
- merge / co-relate
- generate
- calculate
- configure 
### Nouns
- TradeData
- Counter Party
- TDS (External)
- RDS (External)
- Excel (Excel)
- Risk Report
- Risk Parameter

### Actors
- Bussiness User
- TDS System
- RDS System
- Excel Engine
- Scheduler System

### UseCases
 - import RDS Data
 - import TDS Data
- export ExcelRiskreport
- merge / co-relate RiskInput data
- generate RiskReport
- calculate Risk
- configure RiskCalculation
### Subject /  Boundray (module,subsystem,BusinessContext)
- Financial Risk Management System

### Object Oriented Decomposition

## Hierarchy Of OOPs Concepts
#### 1.Encapsulation

- Define Role and Assign Responsibilities
- SRP Principle
	- Class should not change for more than one Reason
	- High Cohesion 
		- inter dependency b/w class members must be tightly coupled
- UML Diagram - Class Diagram

### Candidate Object List 

- XMLDataReader
- XMLTradeDataReader
- XMLRDSDataReader
- RDSDataModel
- TDSDataModel
- RiscCalculator
- RiskConfigrationParameterModel
- RiskReportGenerator
- RiskResultModel
- RiskResultReportModel
- RiskInputDataMerger
- RiskMergedDataModel
- ExcelReportExporter
- FinancialRiskMgmtControlller

### 2.  Reusability
- Types
	- Class Reuse
	- Object Reuse
	
| Class Reuse(is-a) | Object Reuse (has-a) |
|--|--|
|  Static Relationship -Compiletime relationship, Birth(Parent-Child Relationship| Dynamic Relationship (Marriage) |
|Complete Code reuse| Selective Reuse(Contract Based)|
|Inheritance - One role assumes another role A kind of relationship allows us to reuse complete code from another role @compiletime - Complete Code reuse,  Commonality and Variation (family of classes), Generalization and specialization ,  Hierarchy (Single,Multiple,Multilevel,Hybrid) | Uses Relationship : One role uses Another Role (Association,Composition,Aggregation) - Dynamic relationship,No Ripple Effect ,Lazy Instantiation , dynamic Change in Cardinality (Number of Instances),Two way Reuse
|Additive, Child Interface should remain semantically same | test
|Issues: Static Relationship, Ripple Effect , Diamond Problem , One Way Reuse


### Composition and Aggregation (Specific Forms of Uses Relationship)
|  Composition| Aggregation |
|--|--|
|Whole Relationship  |Part-Of relationship  |
|Death Relationship| Lifetime independent|
|Contains|Holds|
|UI, FileSystem|Aggregators (Containers)
|UML - Filled Diamond| UML - Empty- Diamond

## Dependency Inversion Principle
- Loosely coupled Solution
- Object for Change
- Program for interface not for implementation
- High level module should not depend on Low level Module but both should depend on **Abstraction**

#### High level Module
> One who depend on other (Client)
> One uses other object
> An object depending on other object
> **Car** uses Engine , **User** uses Remote ,**Phone** uses Sim-card , **Application** uses Drivers, **ABS** uses speed-sensors

#### Low Level Module
>one who provides service (read,write,log.......)
> Car uses **Engine** , ABS uses **speed-sensors**

### Steps for Abstraction
- Identify Low Level Module
- **Extract**  required **interface** from Low Level Module
- Let Low Level Module **Realize** the extracted  interface
- Identify High Level Module
- Let High Level Module **depends** on reference of Extracted / Required Interface
- At runtime **substitute** or **inject** instance of Low Level Module  to set high level module interface reference.

#### interface
- public view of an object
- interface dictates kind of vocabulary to be used in the dialog b/w two objects
-  Typed Contract (Commitment and expectation)
	- **Method Signatures**
	- Provider Interface 
		- interface provided by service provider(Low Level Module)
		- **How-  one should request for service**
	- Consumer Interface
	- interface provided by consumer (High Level Module)
	- Expectation form High-level module
	- **"Ensure required behavior exist in low level Module"**
	- Data Type
		- Encapsulates Method Signatures
	- Function Pointer / Struct (having function pointers only)
	- Class - pure virtual methods (C++)
	- use interface identifiers (C#, Java)
	- UML - use Class Diagram , annotate with <<-interface->>
	- Interface GuideLines
		- Name Convention  : interface name begin with **I**
		-** "I"** an object who provide service or who realize contract
		-One Can realize/implement any number of interfaces
		- Avoid Fat interfaces - use **Interface Segregation Principle**

### abstract classes and methods
- Code Reuse Allowed
- Instantiation Restricted( information is incomplete / generalized)
- Can have 0 or many abstract methods(template methods)
- Concrete classes (Derived Classes) must implement all the template methods
- c++ (class with protected constructor / at-least one pure virtual method)
- C# / java use abstract identifier
- UMl - use class diagram and label class name in italic font / use stereotype <<-abstract->>
- ex: vehicle (Drive) , Control (paint), Camera (capture), Person ,sensors ,Screen



	





<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3ODY4OTczOTQsNzcxNTM3OTE3LC0xND
I4MTUxNjgzLC05MjgxNzY2MCwxNTM4NDE1OTEsMjM1OTQyMzIz
LDUxOTA4MDc3NywxMTI1NzU5ODEzLDEwNDIyNDMzMjYsLTEzMj
A2MDI0NjQsMjAwNjQyNTcwLDkyMDMxOTMxMSwtNzM2NzAwNDkz
LDIwNzM4MjYzNzMsNDU5NzU4NjA3LDQ0NDMzMzM5LDEzMzk4Nj
I1MzQsODY0MDkwODM0LDE3NTU1ODU1MzQsMzIzNTU2NDE3XX0=

-->