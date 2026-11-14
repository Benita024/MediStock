
# MediStock
### A Batch-Aware Hospital Pharmacy Inventory Management and Decision-Support System

## Overview

MediStock is a web-based hospital pharmacy inventory management and decision-support system designed to improve medicine availability and reduce avoidable inventory wastage.

The system focuses on batch-wise inventory tracking, expiry monitoring, medicine demand forecasting and intelligent replenishment decisions. It aims to help hospital pharmacy operations maintain appropriate stock levels while accounting for changing medicine consumption patterns, supplier lead times and medicine shelf lives.

## Problem Statement

Hospital pharmacies face challenges in maintaining adequate medicine inventory while avoiding stock shortages, overstocking and expiry-related wastage.

Medicine consumption can change over time, while individual batches have different expiry dates and suppliers may have varying delivery lead times. Conventional inventory management approaches may not adequately account for these factors when making replenishment decisions.

MediStock aims to address these challenges through batch-aware inventory management, demand analysis and data-driven replenishment decision support.

## Key Features

- Medicine and supplier management.
- Batch-wise inventory tracking.
- First Expiry, First Out (FEFO) stock management.
- Medicine expiry and low-stock alerts.
- Historical medicine consumption analysis.
- Machine learning-based demand forecasting.
- Statistical demand-shift detection.
- Replenishment recommendations.
- Inventory simulation and performance evaluation.
- Dashboard and analytical reports.

## Research Focus

The research component investigates whether demand-shift detection can improve replenishment decisions for batch-tracked, expiring medicines.

Different replenishment strategies will be evaluated under varying demand conditions, supplier lead times and medicine shelf lives using controlled inventory simulations.

The evaluation will consider medicine availability, stockouts, expiry-related wastage, inventory levels and simulated inventory costs.

## Technology Stack

| Component | Technology |
|---|---|
| Frontend | React.js |
| Backend | Python Flask |
| Database | MongoDB |
| Data Processing | Hadoop, Apache Spark, Pandas, NumPy |
| Machine Learning | Scikit-learn and selected advanced ML algorithms |
| Data Visualisation | Chart.js |
| Cloud Deployment | Amazon Web Services (AWS) |
| Version Control | Git and GitHub |

## Project Scope

The project focuses on hospital pharmacy inventory management and decision support.

It includes batch-level stock tracking, expiry monitoring, demand forecasting, demand-shift detection, replenishment recommendations and inventory simulation.

The initial research experiments will use synthetic demand data and controlled inventory scenarios.

Automated purchasing, live hospital-system integration and actual medicine distribution are outside the current project scope.

## Project Status

**Currently in development.**

The project is being developed incrementally using an Agile approach with lightweight Kanban task tracking.

## Repository Structure

```text
MediStock/
├── backend/
├── frontend/
├── simulation/
├── data/
├── docs/
├── research/
├── tests/
├── README.md
├── DEVELOPMENT_LOG.md
├── PROJECT_BOARD.md
├── CHANGELOG.md
└── .gitignore
```

## Academic Context

Master of Computer Applications (MCA)  
Specialisation: Artificial Intelligence and Data Science

## License

License to be determined.
