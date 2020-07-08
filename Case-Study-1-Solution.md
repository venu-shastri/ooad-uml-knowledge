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

- XMLTradeDataImporter

<!--stackedit_data:
eyJoaXN0b3J5IjpbNDM2NzM3NDk4LDM0ODQyMzQ4MCwxNTI5OT
M2NzAzLDc2MDAwMDY5NiwxODUwODYyNjg5LC0xMjIxOTgwOTk1
LDEzMjQ4Njc0NDJdfQ==
-->