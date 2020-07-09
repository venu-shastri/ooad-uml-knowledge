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
	- interdependency b/w class members must
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


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTkyMjA0ODg5Nyw3MDExODYyNzMsLTE3Nz
I4NzYxNDIsLTIxMDEzNTgzNjQsNjA4MjcxNTIzLDEyNjk1NTg3
OTMsMzQ4NDIzNDgwLDE1Mjk5MzY3MDMsNzYwMDAwNjk2LDE4NT
A4NjI2ODksLTEyMjE5ODA5OTUsMTMyNDg2NzQ0Ml19
-->