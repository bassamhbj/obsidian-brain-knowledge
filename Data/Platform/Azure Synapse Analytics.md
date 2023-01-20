# What is Azure Synapse?
- Enterprise analytics service
- Accelerates insight on data across data warehousing and big data
- Used technologies:
	- SQL for enterprise warehousing 
	- Spark for big data
	- Data Explorer for log and time series analytics 
	- Pipelines for ETL/ELT (same engine as Azure Data Factory)
	- Integration with PowerBI, AML or CosmosDB
![](https://learn.microsoft.com/en-us/azure/synapse-analytics/media/overview-what-is/synapse-architecture.png)

# Synapse SQL
- **Industry leading**
- SQL for query data warehousing and virtualization scenarios 
- Also for data streaming and machine learning 
- Serverless and dedicated resources 
- Streaming data from cloud services to SQL table
- Integrate AI with SQL using native functions: [T-SQL Predict ](https://learn.microsoft.com/en-us/sql/t-sql/queries/predict-transact-sql?view=azure-sqldw-latest&preserve-view=true)

# Apache Spark
- **Industry Standard**
- Open source big data engine. Uses:
	- Data preparation
	- Data engineering 
	- ETL
	- Machine learning 
- ML models with SparkML algorithms and AML integration
- Fast start-up and autoscaling
- Built support for .NET spark (C#)

# Work with Data Lake
- Azure Synapse remove barries between SQL and Spark
- Both can be mixed
- Tables defined on files in the data lake are consumed by Spark or Hive
- SQL and Spark can analyze Parquet, CSV, TSV and JSON
- Scalable data loading between SQL databases and Spark databases

# Data Explorer
- **Preview**
- Query experience for log and telemetry data
- Near real time log analytics and IoT analytics
- Uses
	- Consolidate and correlate logs across on premise, cloud and data source
	- AI Ops (pattern recognition, anomaly detection, forecasting....)
	- Build IoT Analytics solutions
	- Build Analytical SaaS

# Terminology 
| Term | Definition |
| - | - |
| Synapse Workspace | - Azure Resource </br> - Use ADLS Gen2 with file system for temp data | 
| SQL/Spark pool | Computing resources? |
| Linked services | Connection strings for external services |
| Synapse SQL | Ability to do T-SQL based analytics |
| Apache Spark | - Spark Notebooks: For data science (C#, Scala, PyShark, SparkSQL) </br> - Spark Jobs: batch jobs (jar)
| Synapse ML (MMLSpark) | - Library for create ML pipelines </br> - Unifies multiple ML framework </br> - [Key Features]([key features of SynapseML](https://learn.microsoft.com/en-us/azure/synapse-analytics/machine-learning/synapse-machine-learning-library)) |
| Pipelines | - Data Integration (move data and orchestrate) |
| Data Exploter (Preview) | - Analyze insight from log and telemetry data </br> - Data Explorer database are hosted in pools. Tables can br structured or semi structured JSON </br> - External Table: reference table outside Data Explorer. Used for query and export data | 

# Tutorial 
[Get Start Tutorial](https://learn.microsoft.com/en-us/azure/synapse-analytics/get-started)
