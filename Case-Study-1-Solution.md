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
|  Static Relationship -Compiletime relationship, Birth(Parent-Child Relationship| Dynamic Relationship |
|Complete Code reuse| Selective Reuse(Contract Based)|
|Inheritance - A kind of relationship allows us to reuse complete code from another role @compiletime - Complete Code reuse,  Commonality and Variation (family of classes), Generalization and specialization ,  Hierarchy (Single,Multiple,Multilevel,Hybrid) | Uses Relationship : One role uses Another Role (Association,Composition,Aggregation) - Dynamic relationship,No Ripple Effect ,Lazy Instantiation , dynamic Change in Cardinality ,Two way Reuse
|Additive, Child Interface should remain semantically same | test
|Issues: Static Relationship, Ripple Effect , Diamond Problem , One Way Reuseh






<!--stackedit_data:
eyJoaXN0b3J5IjpbMjA3MzgyNjM3Myw0NTk3NTg2MDcsNDQ0Mz
MzMzksMTMzOTg2MjUzNCw4NjQwOTA4MzQsMTc1NTU4NTUzNCwz
MjM1NTY0MTcsNzkwNjAxNDQsOTI3OTMzNTg2LDM4NjU0MTUzOC
wxNDY1NjI0MzEwLDU1MDk5MDY2MSw3MDExODYyNzMsLTE3NzI4
NzYxNDIsLTIxMDEzNTgzNjQsNjA4MjcxNTIzLDEyNjk1NTg3OT
MsMzQ4NDIzNDgwLDE1Mjk5MzY3MDMsNzYwMDAwNjk2XX0=
-->