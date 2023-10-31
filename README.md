# ETL Projet : Call Center analysis

In this project, we reorganized the data of a data center to allow the company to gain a clearer overview of its performance

Receiving a significant volume of calls daily, this information is logged across multiple files, making it challenging to utilize in its current format.

To gain a better understanding of its activity, the company needs the data to be restructured and centralized into a single data warehouse. This will enable more straightforward and efficient analyses.

# Data Pipeline

There will be 3 steps in this process :

STEP 1 : STA The Staging (STA) is used to store the data as we receive them. No modification will be applied.

STEP 2 : ODS The Operational Data Store (ODS) serves as the primary location for data cleansing and normalization. Within this area, all necessary modifications are applied — including merging datasets, adding, or splitting columns, adjusting data types, and more. If any data fails to meet the set quality standards, they will be recorded in a file called "Technical_Rejects". Subsequently, all these technical rejections will be consolidated in an "Administration" (ADM) file.

STEP 3 : DWH The Data Warehouse (DWH) is the final step. It will store all the original data that have been cleaned and restructured. It will be organized like a “Star Schema” , with one Fact Table (“Calls” in this project) and several dimension tables.

# Installation :

- MS SQL Server Visual Studio 

- SSIS module To be able to execute the project , you will need to upload the Zip file and change the server connections (See documentation).

# Documentation

- Convention_name : https://sqlkover.com/ssis-naming-conventions-2-0/

- Guide for executing the ETL project in SSIS & SQL Server : See PDF 'Project SetUp Guide'
