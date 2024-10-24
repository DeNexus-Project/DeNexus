# Data Architecture on Azure: Proposed Architecture for Data Ingestion, Processing, Storage, and Visualization.
This document details the proposed data architecture for **DeNexus**, a company specialising in cybersecurity, with the objective of optimising data ingestion, processing, storage and visualisation, using **Microsoft Azure** cloud services. This architecture is designed to provide a scalable, flexible and robust solution for handling diverse data sources, including web scraping and CSV files, while enabling advanced analytics and reporting.

## Introduction.
This proposed architecture for DeNexus, a company specialising in cybersecurity, is designed to optimise data management using Microsoft Azure cloud services. The solution includes secure data ingestion, efficient data processing, scalable storage and advanced visualisation. The architecture aligns with DeNexus' needs, focusing on scalability, automation and protection of critical data.

## Main scheme.
1. **Data Ingestion.**
Data comes from multiple critical sources and is ingested using secure and scalable methods:
   - Web Scraping.
   - CSV Files.

2. **Data Storage.**
The collected data are stored in secure solutions, guaranteeing durability and controlled accessibility.
   - Azure Data Lake Storage Gen2.
   - Azure Blob Storage.

3. **Data Processing and ETL.**
Data processing is performed in a secure and scalable manner, allowing data transformation for advanced analysis.
   - Azure Data Factory (ADF).
   - Azure Databricks.

4. **Structured Data Storage.**
After processing, the structured data is stored in a secure and highly available database.
   - Azure SQL Database.

5. **Advanced Analytics (Optional).**
To detect patterns and anomalous behaviour in the data, an optional advanced analysis layer is included.
   - Azure Machine Learning.

6. **Data Visualization and Analysis.**
For strategic decision-making, the architecture includes visualisation tools that allow for efficient interpretation of data.
   - External Tools: *Power BI*.

## Conceptual diagram.
The conceptual diagram, developed with PlantUML, presents a clear view of the data flow from ingestion to visualisation.
![UML Architecture](UML\uml-architecture.png)

## Cloud Features.
The proposed architecture for DeNexus leverages several Microsoft Azure services to ensure a scalable, secure and efficient environment. The main features of the cloud services used are described below:
- **Azure Blob Storage** or **Azure Data Lake Storage Gen2.** Cloud storage solutions designed to handle large volumes of unstructured data.
- **Azure Databricks.** Analytics platform based on Apache Spark that enables massive data processing in real time. It offers a solution for transforming, cleansing and analysing large volumes of security data.
- **Azure SQL Database.** A fully managed relational database service. In this architecture, it is used to store processed structured data, ready for analysis and visualisation.
- **Azure Machine Learning.** Integrated environment for developing, training, deploying and managing machine learning models. In the context of DeNexus, it can be used to analyse anomalous behaviour, predict cyber-attacks and create advanced models for threat detection.
- **Azure Data Factory (Basic Pipeline).** Orchestration and automation of data workflows. ADF enables the integration of multiple data sources, such as web scraping and CSVs, and automates ingestion, transformation and loading (ETL) processes. In the DeNexus architecture, ADF ensures that data flows efficiently from initial storage to processing and analysis.
