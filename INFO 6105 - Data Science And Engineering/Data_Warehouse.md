## Multi dimensional Schemas:-
Multidimensional schema is especially designed to model data warehouse systems. The schemas are designed to address the unique needs of very large databases designed for the analytical purpose (OLAP).

# What is OLAP?
Online Analytical Processing, a category of software tools which provide analysis of data for business decisions. OLAP systems allow users to analyze database information from multiple database systems at one time.
>The primary objective is data analysis and not data processing.
## Example of OLAP
Any Datawarehouse system is an OLAP system. Uses of OLAP are as follows

A company might compare their mobile phone sales in September with sales in October, then compare those results with another location which may be stored in a sperate database.
Amazon analyzes purchases by its customers to come up with a personalized homepage with products which likely interest to their customer.

# What is OLTP?
Online transaction processing shortly known as OLTP supports transaction-oriented applications in a 3-tier architecture. OLTP administers day to day transaction of an organization.
> The primary objective is data processing and not data analysis
## An example of OLTP system is ATM center. Assume that a couple has a joint account with a bank. One day both simultaneously reach different ATM centers at precisely the same time and want to withdraw total amount present in their bank account.

However, the person that completes authentication process first will be able to get money. In this case, OLTP system makes sure that withdrawn amount will be never more than the amount present in the bank. The key to note here is that OLTP systems are optimized for transactional superiority instead data analysis.

Other examples of OLTP system are:

> Online banking
> Online airline ticket booking
> Sending a text message
> Order entry
> Add a book to shopping cart

# KEY DIFFERENCE:
1. Online Analytical Processing (OLAP) is a category of software tools that analyze data stored in a database whereas Online transaction processing (OLTP) supports transaction-oriented applications in a 3-tier architecture.
2. OLAP creates a single platform for all type of business analysis needs which includes planning, budgeting, forecasting, and analysis while OLTP is useful to administer day to day transactions of an organization.
3. OLAP is characterized by a large volume of data while OLTP is characterized by large numbers of short online transactions.
In OLAP, data warehouse is created uniquely so that it can integrate different data sources for building a consolidated database whereas OLTP uses traditional DBMS.

# What is ETL?
ETL is defined as a process that extracts the data from different RDBMS source systems, then transforms the data (like applying calculations, concatenations, etc.) and finally loads the data into the Data Warehouse system. ETL full-form is Extract, Transform and Load.

# Following are 3 chief types of multidimensional schemas each having its unique advantages:-

1. Star Schema
Center of the Star can have 1 fact table anda number of associate dimesions. it is known as Star as it resmebles star.
Simplest type of Star Schema
> Characteristics of Star Schema:

>>Every dimension in a star schema is represented with the only one-dimension table.
>>The dimension table should contain the set of attributes.
>>The dimension table is joined to the fact table using a foreign key
>>The dimension table are not joined to each other
>>Fact table would contain key and measure
>>The Star schema is easy to understand and provides optimal disk usage.
>>The dimension tables are not normalized. 

2. Snowflake Schema
Extension of Star Schema and adds additional dimensions. The dimension tables are normalized which splits data into additional tables.

>Characteristics of Snowflake Schema:

>>The main benefit of the snowflake schema it uses smaller disk space.
>>Easier to implement a dimension is added to the Schema
>>Due to multiple tables query performance is reduced
>>The primary challenge that you will face while using the snowflake Schema is that you need to perform more maintenance efforts because of the more lookup tables.


3. Galaxy Schema
A Galaxy Schema contains two fact table that shares dimension tables. It is also called Fact Constellation Schema. The schema is viewed as a collection of stars hence the name Galaxy Schema.
> Characteristics of Galaxy Schema:

>>The dimensions in this schema are separated into separate dimensions based on the various levels of hierarchy.
>>>For example, if geography has four levels of hierarchy like region, country, state, and city then Galaxy schema should have four dimensions.
>>>Moreover, it is possible to build this type of schema by splitting the one-star schema into more Star schemes.
>>The dimensions are large in this schema which is needed to build based on the levels of hierarchy.
>>This schema is helpful for aggregating fact tables for better understanding

# What is a data lake?
A data lake is a centralized repository that allows you to store all your structured and unstructured data at any scale. You can store your data as-is, without having to first structure the data, and run different types of analytics—from dashboards and visualizations to big data processing, real-time analytics, and machine learning to guide better decisions.


Source:- 
1. https://www.guru99.com/star-snowflake-data-warehousing.html
2. https://www.guru99.com/oltp-vs-olap.html