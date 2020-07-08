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

#### Encapsulation
- Define Role and Assign Responsibilities
- SRP Principle
### Candidate Object List 

- XMLTradeDataReader
- XMLRDSDataReader
- RDSDataModel
- TDSDataModel
- Ri
- 

<!--stackedit_data:
eyJoaXN0b3J5IjpbOTYxMzc0NDQwLC0yMTAxMzU4MzY0LDYwOD
I3MTUyMywxMjY5NTU4NzkzLDM0ODQyMzQ4MCwxNTI5OTM2NzAz
LDc2MDAwMDY5NiwxODUwODYyNjg5LC0xMjIxOTgwOTk1LDEzMj
Q4Njc0NDJdfQ==
-->