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
	
| Class Reuse | Object Reuse |
|--|--|
|  Static Relationship -Compiletime relationship| Dynamic Relationship |
|Complete Code reuse|Test|
|Inheritance - A kind of relationship allows us to reuse complete code from another role @compiletime - Complete Code reuse,  Commonality and Variation (family of classes), Generalization and specialization ,  Hierarchy (Single,Multiple,Multilevel,Hybrid) | NewTest 
|Additive, Child Interface should remain semantically same | test
|Limitations: Static Relationship, Ripple Effect






<!--stackedit_data:
eyJoaXN0b3J5IjpbODY0MDkwODM0LDE3NTU1ODU1MzQsMzIzNT
U2NDE3LDc5MDYwMTQ0LDkyNzkzMzU4NiwzODY1NDE1MzgsMTQ2
NTYyNDMxMCw1NTA5OTA2NjEsNzAxMTg2MjczLC0xNzcyODc2MT
QyLC0yMTAxMzU4MzY0LDYwODI3MTUyMywxMjY5NTU4NzkzLDM0
ODQyMzQ4MCwxNTI5OTM2NzAzLDc2MDAwMDY5NiwxODUwODYyNj
g5LC0xMjIxOTgwOTk1LDEzMjQ4Njc0NDJdfQ==
-->