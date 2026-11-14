
# MediStock — Software Requirements

## 1. Purpose

This document defines the functional and non-functional requirements of MediStock, a batch-aware hospital pharmacy inventory management and decision-support system.

## 2. Functional Requirements

### FR-01: Medicine Management
- The system shall allow users to add, view, update and manage medicine records.
- Each medicine shall have details such as name, category, unit and other relevant attributes.

### FR-02: Supplier Management
- The system shall maintain supplier information.
- Users shall be able to associate suppliers with medicines and their supply details.

### FR-03: Batch-wise Inventory Management
- The system shall maintain individual batch records for each medicine.
- Each batch shall include quantity, batch number, manufacturing date and expiry date.
- The system shall record stock additions and issues.

### FR-04: FEFO-based Stock Management
- The system shall support the First Expiry, First Out (FEFO) principle.
- Stock from batches with earlier expiry dates shall be prioritised during issue.

### FR-05: Expiry and Low-stock Monitoring
- The system shall monitor medicine batch expiry dates.
- The system shall generate alerts for medicines approaching expiry.
- The system shall identify medicines whose stock falls below defined thresholds.

### FR-06: Demand Analysis and Forecasting
- The system shall maintain historical medicine consumption data.
- The system shall analyse consumption patterns.
- The system shall generate future demand estimates using machine learning techniques.

### FR-07: Demand-shift Detection
- The system shall analyse medicine consumption patterns to identify significant demand changes.
- Statistical change-detection techniques shall be evaluated for identifying sudden or gradual demand shifts.

### FR-08: Replenishment Decision Support
- The system shall generate replenishment recommendations using inventory levels, forecast demand and relevant demand changes.
- Recommendations shall account for supplier lead times and medicine shelf life.

### FR-09: Inventory Simulation and Evaluation
- The system shall support controlled inventory simulations using configurable demand scenarios.
- The system shall evaluate different replenishment strategies.
- Performance shall be compared using stockout, medicine availability, expiry wastage, inventory and cost-related metrics.

### FR-10: Big Data Processing
- The system shall use Hadoop for distributed storage of historical datasets.
- The system shall use Apache Spark for processing and analysing historical medicine consumption data.
- MongoDB shall maintain operational application data and inventory records.

### FR-11: Dashboard and Reporting
- The system shall provide a dashboard displaying relevant inventory information.
- The system shall present demand forecasts, alerts and replenishment recommendations.
- The system shall provide analytical summaries and simulation results.

### FR-12: Cloud Deployment
- The application shall be deployed on Amazon Web Services (AWS).
- The deployed application shall be accessible through a web browser.

## 3. Non-Functional Requirements

### NFR-01: Usability
- The system shall provide a clear and user-friendly interface.
- Important inventory information and alerts shall be easy to understand.

### NFR-02: Performance
- Common inventory operations shall execute within reasonable response times.
- Data processing and simulation tasks shall be designed to handle the intended project datasets.

### NFR-03: Reliability
- The system shall maintain consistency of inventory and batch records.
- Invalid stock operations shall be prevented through appropriate validation.

### NFR-04: Security
- The system shall provide appropriate access controls.
- Sensitive configuration details and credentials shall not be exposed.

### NFR-05: Maintainability
- The application shall use a modular architecture.
- Code and project documentation shall be maintained in a structured manner.

### NFR-06: Scalability
- The data-processing architecture shall support larger historical datasets as the system evolves.

## 4. Project Constraints and Limitations

- Initial research experiments shall use synthetic demand and inventory data.
- The system is intended as a prototype and decision-support tool, not a replacement for professional pharmacy operations.
- Automated purchasing and actual medicine distribution are outside the project scope.
- Live integration with hospital information systems is not included.
- Simulation results shall be interpreted within the assumptions and scenarios tested.

## 5. Requirement Status

The requirements in this document represent the initial planned system specifications. They may be refined following technical design, subject-project requirements and implementation feasibility reviews.
