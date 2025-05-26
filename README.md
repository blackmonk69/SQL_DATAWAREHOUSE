# SQL_DATAWAREHOUSE

In this project we build a datawarehouse with the help of some csv files, MSSQL Server, Python. The whole idea is to show an ETL process where the data architecture is organized in layers (bronze, silver and gold) known as Medallion Architecture, and the data after wrangling is injected into a DB in MSSQL Server.

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.


This project involves:

1. **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.

Note: Regarding naming conventions we decided to use: nameoflayer_sourcesystem_nameoffile

The part where we load the data from the csv into the tables in the bronze Layer is critical, we have to make sure there is a 100% match after performing the bulk insert, which by the way means inserting data in a massive way all at once.
By referring to a 100%match I mean exact correspondence between name fields and the content of the table. 







