# Project: Data Warehouse

## Project Description
In this project we will create a Redshift DB with user activity and songs. The data will be loaded from S3 bucket that contains JSON files.
Once data is loaded and transformed into dimensional tables we can run the sql queries to find insights for our interest.

## Project Files Description

- dwh.cfg - contains the info for redshift database and IAM role 
- create_cluster.py - it will drop and create the fact and dimension tables empty in the Redshift DB
- etl.py - it will load data from S3 into staging tables on Redshift and then process that data into the analytics tables on Redshift.
- sql_queries.py - it contains the definition for the SQL statements: create table DDLs, the insert statements and copy commands.


## Project Files Execution

Steps that were done to complete this project:
- Create the IAM role whcih had assigned: AmazonS3ReadOnlyAccess and AmazonRedshiftAllCommandsFullAccess
- Create the security group that authorise redshift cluster acces
- Create the Redshift cluster

