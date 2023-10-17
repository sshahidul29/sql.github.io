## Overview

This project's main goal is to help our retail client use data for better decision-making. We'll build a strong data system that includes an Operational Data Store (ODS) and a Data Warehouse. This project includes the tasks of combining, refining, and organizing data, developing analytical models, and showcasing the outcomes in a user-friendly manner using data visualizations and dashboards.

## Enterprise Data Warehouse was built in MSSQL Server using SSMS
- Led complete database lifecycle management including installation, upgrade, troubleshooting, migration, and security.
- Conducted stakeholder analysis and requirements gathering sessions, aligning data with business needs.
- Designed Conceptual and Logical data models for the OLTP Operational Data Store (ODS) and implemented Physical Data models using Bill Inmon’s Relational Modeling Techniques in the MSSQL Server using SSMS. 
- Created Bus Matrix (composition of Business process, Granularity, Facts, Fact Tables, and Dimensions).
- Designed and implemented Enterprise Data Warehouse (EDW) using Ralph Kimball’s Dimensional Modelling Approach.
- Created and configured Staging, EDW, and Control Framework databases on MS SQL Server. 

  ![Purchase Analysis](https://github.com/sshahidul29/Supply-Chain-Data-Modernization/blob/main/Figures/SCODS.PNG)  

Figure 1: OLTP Operational Data Store (ODS) using Bill Inmon’s Relational Modeling Techniques (3NF).

  ![Purchase Analysis](https://github.com/sshahidul29/Supply-Chain-Data-Modernization/blob/main/Figures/SCODS.PNG)  

Figure 2: Enterprise Data Warehouse using Ralph Kimball’s Dimensional Modelling Approach.

## ETL Pipeline was built in Visual Studio using SSIS

- The project aimed to create an ETL (Extract, Transform, Load) pipeline for data extraction, transformation, and loading into SQL Server Databases from the OLEDB source.
- Wrote ETL packages to extract, transform and load data from the OLEDB source to Staging and staging to EDW Databases.
- Created a metric table for an audit of Source Count, and Destination Count Staging database, and Pre, Current, Post, Type1, and Type2 Counts for EDW using the Control framework database.
- Implemented server agent for automated data loading and scheduling.

  
  ![Sales Analysis](https://github.com/sshahidul29/Sales-and-Procurement-Data-Integration-and-Analytics-Framework/blob/main/Figures/SalesCETL.PNG)

 Figure 2: Control-flow diagram for ETL Pipeline

  ![Sales Analysis](https://github.com/sshahidul29/Sales-and-Procurement-Data-Integration-and-Analytics-Framework/blob/main/Figures/Product.PNG)

 Figure 3: Data-flow diagram of ETL Pipeline for Product dimension

 ![Sales Analysis](https://github.com/sshahidul29/Sales-and-Procurement-Data-Integration-and-Analytics-Framework/blob/main/Figures/SalesETL.PNG)

Figure 4: Data-flow diagram for Incremental load of ETL Pipeline for Factsales

![Sales Analysis](https://github.com/sshahidul29/Sales-and-Procurement-Data-Integration-and-Analytics-Framework/blob/main/Figures/Control.PNG)

Figure 5: Control-flow diagram for ETL Pipeline to automate the system through SQL Server Agent

## Datamart was built using SSAS for Business Users

- Cubes were built using SQL Server Analysis Services (SSAS) for multi-dimensional and Tabular analysis for business users. These cubes supported interactive dashboards and data visualizations for informed decision-making.

 ![Sales Analysis](https://github.com/sshahidul29/Sales-and-Procurement-Data-Integration-and-Analytics-Framework/blob/main/Figures/SalesM.PNG)

Figure 6: Sales Cube for Multidimensional Analysis

 ![Sales Analysis](https://github.com/sshahidul29/Sales-and-Procurement-Data-Integration-and-Analytics-Framework/blob/main/Figures/salesTab.PNG)

Figure 7: Sales Cube for Tabular Analysis

![Sales Analysis](https://github.com/sshahidul29/Sales-and-Procurement-Data-Integration-and-Analytics-Framework/blob/main/Figures/PurchaseM.PNG)

Figure 8: Purchase Cube for Multidimensional Analysis

 ![Sales Analysis](https://github.com/sshahidul29/Sales-and-Procurement-Data-Integration-and-Analytics-Framework/blob/main/Figures/PurchaseTab.PNG)

Figure 9: Purchase Cube for Tabular Analysis
