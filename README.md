Name:  SOHogan


Date:  Nov 30, 2022


Course:  IT FDN 130 A Au 22: Foundations Of Databases & SQL Programming


Github URL:  https://github.com/seanpo206/Module7 

# Assignment 7 – DB Foundation

## Introduction
According to dotnettricks.com: 


* *“A function is a database object in SQL Server. Basically, it is a set of SQL statements that accept only input parameters, perform actions and return the result. The function can return only a single value or a table. We can't use a function to Insert, Update, Delete records in the database table(s)” (https://www.dotnettricks.com/learn/sqlserver/different-types-of-sql-server-functions#:~:text=A%20function%20is%20a%20database,the%20database%20table(s)), Nov, 2022* *


A function allows us to do more with data than just query it.  We can actually do things with the data, such as find the average, mean, or sum of integers.   We can concatenate, format, trim and apply if-then logic.  
There are two types of functions.   They are listed below:
1.	Aggregate:  Are functions that operate on many records and spit out a summary.
2.	Non-Aggregate:  Are functions that operate on each record independently.
Functions produce one of the two following types of resulting values:
1.	Single-valued (produce a single alphanumeric value.  Are also most common.)
2.	Table-valued (produce many results that are displayed within a table.)
There are two major categories of functions:
1.	System Defined Functions (SDF):  These are predefined functions that come standard already apart of the database query language.
2.	User Defined Functions (UDF):  These are specialized functions that are created and then used by the end user.
When to Use a SQL UDF
Since the SQL query language has already built-in functions, UDFs are intended for specialized function development during times when SDFs don’t meet the specific requirements of the results one hopes to achieve.  Due to the complexity of data analysis, there are times when the standard array of built-in functions aren’t enough.  
## The Difference Between Scalar, Inline and Multi-Statement Functions
There are three classifications of functions.  They are listed below:
1.	Scalar
2.	Inline
3.	Multi-Statement
Scaler Functions: Return only a single value which is mandatory.  A scaler function can return any type of data except text, ntext, image, cursor or timestamp.
Inline Functions: Are a table-valued function.  Multiple values are returned in the form of a table.  Part of the syntax of this function requires you to identify the name of the output table.   Additionally, unlike a scaler function, an inline function uses a single SELECT statement (to return a single table) and thus does not need a BEGIN and END block.
Multi-Statement Functions: Similar to an inline function in that it will return multiple values in the form of a table with two differences.  One, multi-statement functions can use more than one SELECT statement.  Two, the multi-statement function has flexibility to customize the resulting table whereas the inline function is limited to the functionality of it’s single SELECT statement. 

## Summary
Functions are database query tools that allow data to be further manipulated other than a simple query statement.  There are two types of functions, aggregate (many records, summary of results) and non-Aggregate (operate on many records each independent).  There are two types of function results, single-valued and table-valued.   There are two major categories of functions, System Defined Functions(SDF)(built in standard functions) and User Defined Functions(UDF)(User custom designed functions).  When a user has data analysis needs that can’t be met by SDFs, then that user can develop a UDF to better meet more specific data analysis needs.
