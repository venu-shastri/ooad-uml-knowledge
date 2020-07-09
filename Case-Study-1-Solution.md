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
|Inheritance - A kind of relationship allows us to reuse complete code from another role @compiletime - Complete Code reuse,  Commonality and Variation (family of classes), Generalization and specialization ,  Hierarchy | NewTest 
|Additive, Child Interface should remain semantically same | test
|Limitations: Static Relationship, Ripple Effect






<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc1NTU4NTUzNCwzMjM1NTY0MTcsNzkwNj
AxNDQsOTI3OTMzNTg2LDM4NjU0MTUzOCwxNDY1NjI0MzEwLDU1
MDk5MDY2MSw3MDExODYyNzMsLTE3NzI4NzYxNDIsLTIxMDEzNT
gzNjQsNjA4MjcxNTIzLDEyNjk1NTg3OTMsMzQ4NDIzNDgwLDE1
Mjk5MzY3MDMsNzYwMDAwNjk2LDE4NTA4NjI2ODksLTEyMjE5OD
A5OTUsMTMyNDg2NzQ0Ml19
-->