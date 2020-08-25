# DBFoundations-Module07
Janet Fisher

August 23, 2020

Foundations of Databases

Assignment 07

# User Defined Functions

## Introduction

According to Wikipedia, “A user-defined function (UDF) is a function provided by the user of a program or environment, in a context where the usual assumption is that functions are built into the program or environment.” (https://en.wikipedia.org/wiki/User-defined_function, 2020). Put simply, UDFs are programming routines that accept parameters, perform actions, and return their results as values. This paper will focus on three types of UDFs: Scalar, Inline, and Multi-Statement. 

## When to Use User Defined Functions (UDFs)
Using SQL, there are several situations that justify the use of UDFs. Here are some guidelines as to when to use them:

- When we do not want to write the same logic over and over

- When we want to reduce the amount of compilation time of the query

- When we need help separating complex calculations from the basic query

- When we want to reduce network traffic

- When we want to limit the number of rows via the Where clause
 
## The Differences between Scalar, Inline, and Multi-Statement Functions
There are three types of UDFs in SQL. They are Scalar functions, Inline table-valued functions, and Multi-Statement table-valued functions. Here are their definitions:

**Scalar Functions**: A scalar function accepts any number of parameters and returns a single item result. The term “scalar” differentiates a single value from more complex structured values, like arrays or result sets.  Scalar functions are more like traditional functions using ordinary programming language.

**Inline (Table-Valued) Functions**: An inline table-valued function returns a result set more like a view. The difference is that this function can accept parameters. The inline function's syntax is simple. The return type is set to a table and the return statement also uses a Select statement in parenthesis. Finally, the table keyword is specified in the return clause.

**Multi-Statement Table-Valued Functions (MSTVFs)**: Multi-Statement functions also return a result set, like Inline UDFs, however, they can be used to perform some differentiated actions outside the context of a standard SELECT statement. An MSTVF can create a temporary table, delineating the fields, as well as their type and characteristics. To return the result set, script also needs to be constructed. The purpose here is to achieve either of two results: either to process some unique form of business logic by assembling a virtual table, or to replicate the functionality of the inline function in a more elaborate and better-compiled format. 


## Summary
UDFs are powerful tools. They should be used when a calculation will be repeated multiple times, for example: calculating a tax on different products based on already-established rules that are subject to change over time. UDFs are not difficult to use and maintain, however during this research, there seemed to be many warnings regarding their use, especially if the user is not an expert. Multi-statement table-valued functions especially seem to be problematic for those who are not well aquainted with them.

## References:
https://www.youtube.com/playlist?list=PLfycUyp06LG_8aYt19coVTwUDr2CaaSY5, 2020

http://www.paladn.com/resources/links-and-tools/122.html,2020

https://www.sqlservertutorial.net/sql-server-user-defined-functions/sql-server-table-valued-functions/, 2020

https://aboutsqlserver.com/2011/10/23/sunday-t-sql-tip-inline-vs-multi-statement-table-valued-functions/, 2020

https://database.guide/difference-between-multi-statement-table-valued-functions-inline-table-valued-functions-in-sql-server/, 2020

https://social.msdn.microsoft.com/Forums/sqlserver/en-US/e8aaefdb-0269-437f-b352-, 2020

https://www.techrepublic.com/blog/the-enterprise-cloud/understand-when-to-use-user-defined-functions-in-sql-server/, 2020

https://www.sqlshack.com/learn-sql-user-defined-functions/, 2020

https://docs.microsoft.com/en-us/sql/relational-databases/user-defined-functions/create-user-defined-functions-database-engine?view=sql-server-ver15, 2020

https://www.red-gate.com/simple-talk/sql/t-sql-programming/sql-server-user-defined-functions/, 2020
