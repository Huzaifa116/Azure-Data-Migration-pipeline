# Azure-Data-Migration-pipeline

## Architecture Diagram

![Azure Architecture diagram](https://github.com/Mehmaam99/Azure-Data-Migration-Pipeline/assets/45142408/b3e93058-6d1d-481c-89e3-2a300e44f4a2)

## Overview

This project covers end-to-end migration of an on-premises SQL Server database to Azure Synapse Analytics. The migration process involves three main steps:

1. Data Ingestion
2. Data Transformation  
3. Data Loading

## Prerequisites

- On-premises SQL Server with sample database
- Azure subscription
- Azure Data Factory
- Azure Data Lake Gen2
- Azure Databricks
- Azure Synapse Analytics

## Data Ingestion

- Install and configure on-premises SQL Server with AdventureWorksLT sample database
- Create Azure Data Factory instance
- Create Azure Data Lake Gen2 storage account  
- Set up self-hosted integration runtime to connect on-prem SQL Server with Data Factory
- Create pipeline to copy tables from on-prem SQL Server to Data Lake Gen2 storage using self-hosted integration runtime

## Data Transformation

- Create Azure Databricks workspace
- Configure access from Databricks to Data Lake Gen2 storage
- Develop Spark notebook for transforming data 
- Add Databricks notebook activity in Data Factory pipeline to run data transformation

## Data Loading 

- Create Azure Synapse Analytics workspace and SQL database
- Develop SQL stored procedure script to create views for tables
- Configure linked service in Data Factory to connect to Synapse SQL database
- Add stored procedure activity in pipeline to create views for transformed tables in Synapse

## Summary

This covers the end-to-end process of migrating an on-premises SQL Server database to Azure Synapse Analytics using Azure Data Factory, Data Lake Gen2, Databricks, and other Azure services. The key steps are ingesting data, transforming it, and then loading it into the target database.


## Note

To follow a detailed process, refer to the PDF document provided in the repository.
