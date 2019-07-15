What is a database?
Large order collection of data.

What is DBMS?
Software that **stores**, manages and facilitates access to data

When people ask about Database, they often confuse it with what?
DBMS

What is origin of DB Symbol?
Looks like first commercial Disk Drive! 5MB 1ton

Relational Terminology:

What is database?
Set of named Relation?

Relation is often called?
Table?

What are 2 parts of Relation?
- Schema
- Instance

What is Relation Schema?
Description or metadata of relation

What is instance of relation?
Set of data in db that satisfying the schema

What is Attribute of relational table?
Column or field, has schema & instance

What is a tuple in Relation?
Record or a row

In SQL every All the types of columns are atomic
All the attribute names are unique

What dose it mean a instance can support multiset of 'rows'(tuples)


SQL C3
How many sublanguages SQL contains?
2

What are Sublanguages of SQL?
Data Definition Lanugage & Data Manipulation Language

What do we need DDL?
define & modify schema

What do we need DML?
Instance manipulation, query, insert, delete, update


## Order BY?

What dose ORDER BY clause do?
Output should be sorted in lexicographic ordering
https://youtu.be/r-4Xj2Fz6MQ?t=131


What is the meaning of the 3 constrains?
`ORDER BY S.gpa, S.name, a2;`
https://youtu.be/r-4Xj2Fz6MQ?t=131
It will order it by gpa, and if tie, brake the tie with next

What is lexicographic ordering?
First filed is ORDER BY is for sort order, and for ties we reverts for second
field and so on
https://youtu.be/r-4Xj2Fz6MQ?t=150

How to ORDER BY columns we're computing?
Using AS clause in select list
```sql
  SELECT S.name, S.gpa, S.age*2 AS a2
  FROM Students S
  ORDER BY a2;
```
https://youtu.be/r-4Xj2Fz6MQ?t=164

## Limit
What will happen here?
```sql
  SELECT S.name, S.gpa, S.age*2 AS a2
  FROM Students S
  WHERE S.dept = 'CS'
  LIMIT 3;
```
Its non-deterministic, you'll get some 3 rows from table
https://youtu.be/r-4Xj2Fz6MQ?t=248


What is important aspect of relations?
They are not in any particular order
https://youtu.be/r-4Xj2Fz6MQ?t=266

## Aggregates

What are aggregate fn?
fn that accept batch of values from a column and using some arithmetic expression
produces result.
https://youtu.be/n2tuTtgkSlI?t=15

What aggregate fn takes as input?
batch of tuples (values from a column)
https://youtu.be/n2tuTtgkSlI?t=16

What aggregate fn produces?
Single value 
https://youtu.be/n2tuTtgkSlI?t=69

Aggregate fn uses what to produces result?
Uses some arithmetic expression
SUM, COUNT, MAX
https://youtu.be/n2tuTtgkSlI?t=18

## GROUP BY

What dose GROUP BY do?
Partition table into groups with same GROUP BY Column val
https://youtu.be/n2tuTtgkSlI?t=117

Group by accept what as argument?
Single column or column list
https://youtu.be/n2tuTtgkSlI?t=124

What GROUP BY produces?
Aggregate result per group

## HAVING

https://youtu.be/n2tuTtgkSlI?t=175

What is HAVING?
It's a clause that filter out unwanted Groups
https://youtu.be/n2tuTtgkSlI?t=174

When Having is Apply?
After group and aggregations
https://youtu.be/n2tuTtgkSlI?t=199

What HAVING accept as input?
anything that can go in SELECT
https://youtu.be/n2tuTtgkSlI?t=215

When we can use HAVING?
Only used in aggregate queries
https://youtu.be/n2tuTtgkSlI?t=224


