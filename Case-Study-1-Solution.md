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
	
| Class Reuse | Object Reuse |
|--|--|
|  Static Relationship -Compiletime relationship, Birth(Parent-Child Relationship| Dynamic Relationship |
|Complete Code reuse|Test|
|Inheritance - A kind of relationship allows us to reuse complete code from another role @compiletime - Complete Code reuse,  Commonality and Variation (family of classes), Generalization and specialization ,  Hierarchy (Single,Multiple,Multilevel,Hybrid) | NewTest 
|Additive, Child Interface should remain semantically same | test
|Issues: Static Relationship, Ripple Effect , Diamond Problem






<!--stackedit_data:
eyJoaXN0b3J5IjpbLTYzNzk0MzQwNSw0NDQzMzMzOSwxMzM5OD
YyNTM0LDg2NDA5MDgzNCwxNzU1NTg1NTM0LDMyMzU1NjQxNyw3
OTA2MDE0NCw5Mjc5MzM1ODYsMzg2NTQxNTM4LDE0NjU2MjQzMT
AsNTUwOTkwNjYxLDcwMTE4NjI3MywtMTc3Mjg3NjE0MiwtMjEw
MTM1ODM2NCw2MDgyNzE1MjMsMTI2OTU1ODc5MywzNDg0MjM0OD
AsMTUyOTkzNjcwMyw3NjAwMDA2OTYsMTg1MDg2MjY4OV19
-->