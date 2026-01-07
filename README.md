# End-to-End Streaming Data Engineering Pipeline

## Overview
This project demonstrates a customized end-to-end data engineering pipeline focused on real-time data ingestion, distributed processing, and scalable storage. The pipeline ingests user event data from a public API, streams it using Apache Kafka, processes and enriches it using Apache Spark, and stores the transformed data in Apache Cassandra. Apache Airflow is used to orchestrate and automate the entire workflow.

This project is **adapted from an open-source data engineering architecture** and customized for academic learning and practical understanding of modern data systems.

---

## Architecture

Public API
↓
Apache Airflow
↓
Apache Kafka
↓
Apache Spark
↓
Apache Cassandra

yaml
Copy code

### Components
- **Data Source**: Public API used to simulate real-time user event data  
- **Apache Airflow**: Orchestrates data ingestion and workflow scheduling  
- **Apache Kafka**: Handles real-time data streaming  
- **Apache Spark**: Processes and transforms streaming data  
- **Apache Cassandra**: Stores processed data in a scalable distributed database  
- **Docker & Docker Compose**: Containerizes and manages all services  

---

## Key Features
- End-to-end real-time data pipeline design  
- Event-based data streaming using Kafka  
- Distributed data processing with Spark  
- Workflow orchestration using Airflow  
- Scalable storage using Cassandra  
- Fully containerized environment  

---

## Customizations Made
The following customizations were applied to better understand the system and demonstrate ownership:

- Renamed Kafka topic to an event-based naming convention  
- Added a derived column during Spark data transformation  
- Updated Cassandra schema to align with processed data  
- Refined project documentation and architecture explanation  

---

## Technologies Used
- Python  
- Apache Airflow  
- Apache Kafka  
- Apache Spark  
- Apache Cassandra  
- PostgreSQL  
- Docker & Docker Compose  

---

## Learning Objectives
- Understand how modern data engineering pipelines are designed  
- Learn real-time data ingestion and streaming concepts  
- Apply Spark transformations on streaming data  
- Explore workflow orchestration with Airflow  
- Gain hands-on exposure to distributed systems  

---

## Getting Started

### Prerequisites
- Docker Desktop  
- Docker Compose  
- Git  

### Run the Project
```bash
docker-compose up
Once the services are running:

Airflow UI: http://localhost:8080

Kafka, Spark, and Cassandra run inside Docker containers

Project Scope
This project focuses on architecture understanding, data flow, and system integration rather than production deployment. Components were studied, adapted, and tested locally to strengthen data engineering fundamentals.

Disclaimer
This project is adapted from an open-source reference for educational purposes. The implementation has been modified to reflect personal learning, experimentation, and documentation improvements.