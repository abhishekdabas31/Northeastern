## Multi dimensional Schemas:-
Multidimensional schema is especially designed to model data warehouse systems. The schemas are designed to address the unique needs of very large databases designed for the analytical purpose (OLAP).

Following are 3 chief types of multidimensional schemas each having its unique advantages:-

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




Source:- 
https://www.guru99.com/star-snowflake-data-warehousing.html