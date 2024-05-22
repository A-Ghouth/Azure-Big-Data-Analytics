WCD Big Data Engineering Capstone Project
Project Overview
The objective of this project is to use big data analytics systems to process data and train a machine learning classifier. Daily posts are processed and passed through an ML classifier to predict their tags.

Project Architecture
The project utilizes the following Azure resources:

Azure Data Factory: Used to create and orchestrate an ETL pipeline, extracting data from the sources, transforming it, and loading it into a data lake.
Azure Monitor: Used to monitor any failures in the ADF pipelines and create email alerts.
Azure Key Vault: Used to store secrets (passwords & access tokens) safely and effectively.
Azure Data Lake Gen2: Used to store raw data initially (landing zone), then store the transformed data for analysis.
Azure Databricks: Used to process the data using Spark's distributed computing power. Spark ML was also used to train and deploy a classifier.
Azure Synapse Analytics: Used for data analysis, querying data from the data lake and creating simple charts.
Data Sources
The data used in this project consists of Stack Overflow posts, post types, and users. The data is ingested from two external sources:

Amazon RDS PostgreSQL DB
Azure Blob Storage
Getting Started
To set up the project, follow these steps:

Provision the required Azure resources.
Configure the data sources and connections in the Azure services.
Implement the ETL pipeline in Azure Data Factory.
Process the data and train the machine learning classifier in Azure Databricks.
Analyze the data and create visualizations in Azure Synapse Analytics.
