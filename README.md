# Retail Store Data Modeling and Analysis using DataStage
## Project Overview:
The project implements a star-schema data warehousing flow, then utilize IBM InfoSphere DataStage to develop efficient ETL (Extract, Transform, Load) pipelines to create data marts and perform some analysis on them.
The objective is to store and analyze data from a fictional retail store in a star-schema-based analysis data warehouse while ensuring all changes in the dimensions are preserved.

## Data Source:
The store's online transaction processing (OLTP) system serves as the primary data source for populating the star schema.
![model](https://github.com/MarinaFawzy/Retail-Store-Data-Modeling-and-Analysis/assets/89097013/87a82cac-9ec4-4cee-ad82-057d37e6228c)

## Project Steps:
1-Physical Data Model Construction: Utilizing UML notation, the star schema comprises three dimensions—product, retail, and customer—alongside a fact table named transactions.

2-Data Extraction: Extract pertinent data from the data warehouse, ensuring comprehensive inclusion of customer, store, and product details.

3-Data Transformation: Apply necessary transformations to the extracted data to ensure alignment with business requirements. One such transformation involves converting customer name columns to uppercase.

4-Data Mart Establishment: Develop a data mart titled RETAIL_DATA_MART, containing transaction records for each customer categorized by customer type ("citizen" or "foreign"), product information, and purchased stock.

5-Data Loading: Load the transformed data into the RETAIL_DATA_MART data mart.

6-Data Mart Analysis: Utilize the RETAIL_DATA_MART data mart to address specific business needs, such as:
    Displaying the transaction count for each employee in every store.
    Identifying the customer type ("citizen" or "foreign") generating the highest profit. For instance, if "foreign" customers conduct 5 transactions and "citizen" 
    customers conduct 3 transactions, the maximum profit would be attributed to foreign customers.
    Granting a bonus to the customer(s) contributing the most to the profit.

## Project Files:
Jobs: contains the dsx file for the DataStage jobs
Dataset: contains the data after it is modeled in a star schema data warehouse model.
JobScreenshot: A visual representation of a DataStage jobs



