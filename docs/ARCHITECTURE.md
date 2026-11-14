
# MediStock — System Architecture

## 1. Architecture Overview

MediStock will follow a modular web application architecture. The system will separate the user interface, backend business logic, operational database, data-processing components and intelligent decision-support modules.

The components will communicate through defined interfaces to support maintainability, testing and future extensions.

## 2. Architectural Components

### 2.1 Frontend Layer
**Technology: React.js**

Responsibilities:
- Display the MediStock dashboard.
- Provide interfaces for medicine, supplier and batch management.
- Display inventory alerts and expiry information.
- Present demand forecasts and replenishment recommendations.
- Visualise analytical and simulation results.

### 2.2 Backend Layer
**Technology: Python Flask**

Responsibilities:
- Handle frontend requests through REST APIs.
- Implement application business logic.
- Manage medicine, supplier and inventory operations.
- Communicate with MongoDB.
- Coordinate forecasting, demand detection and simulation operations.
- Provide data to the frontend.

### 2.3 Operational Database Layer
**Technology: MongoDB**

Responsibilities:
- Store medicine records.
- Maintain supplier information.
- Store batch-wise inventory records.
- Maintain stock transactions.
- Store relevant application and analytical records.

### 2.4 Data Processing Layer
**Technologies: Hadoop HDFS and Apache Spark**

Responsibilities:
- Store historical pharmacy datasets using Hadoop HDFS.
- Process historical medicine consumption data using Apache Spark.
- Perform large-scale data analysis.
- Prepare processed datasets for forecasting and analytical operations.

### 2.5 Intelligence and Decision-Support Layer
**Technologies: Python, Pandas, NumPy, Scikit-learn and selected ML libraries**

Responsibilities:
- Analyse historical medicine consumption.
- Generate medicine demand forecasts.
- Detect significant demand shifts using statistical methods.
- Generate replenishment recommendations using inventory and demand information.

### 2.6 Simulation Layer
**Technology: Python**

Responsibilities:
- Simulate medicine inventory behaviour under different demand conditions.
- Model supplier lead times and medicine shelf lives.
- Implement and compare replenishment strategies.
- Evaluate inventory performance using defined metrics.

### 2.7 Cloud Deployment Layer
**Platform: Amazon Web Services (AWS)**

Responsibilities:
- Host the web application.
- Provide access to the deployed application through a web browser.
- Support the deployment of the required application components.

## 3. Component Interaction

1. Users interact with MediStock through the React frontend.
2. Frontend requests are sent to the Flask backend through REST APIs.
3. The backend retrieves and updates operational records in MongoDB.
4. Historical datasets are stored in Hadoop HDFS and processed using Apache Spark.
5. Processed data is used by the intelligence layer for forecasting and analysis.
6. Demand forecasts and detected changes contribute to replenishment recommendations.
7. The simulation engine evaluates replenishment strategies under controlled scenarios.
8. Results are presented through the dashboard and reporting interfaces.
9. The application will be deployed on AWS.

## 4. Architectural Approach

The system will use a modular architecture with clearly separated responsibilities.

The frontend, backend, data processing, intelligence and simulation components will be developed and tested independently before integration.

The initial implementation will prioritise a manageable application structure rather than introducing unnecessary distributed services.

## 5. Deployment Approach

The application is planned to be deployed on Amazon Web Services (AWS).

The deployment architecture and hosting services will be finalised during the cloud implementation phase after evaluating technical requirements and available resources.

## 6. Architecture Status

This document describes the proposed initial architecture. Component interfaces, data flows and deployment details will be refined during implementation.
