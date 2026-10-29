* **Attribute:** A characteristic or quality of data used to label a column in a table.
* **Observation:** All of the attributes for something contained in a row of a data table.
* **Formula:** A set of instructions that performs a specific action using the data in a spreadsheet.

## Important links
[Google Sheets Training and Help](https://support.google.com/a/users/answer/9282959?visit_id=637361702049227170-1815413770&rd=1)

### SQL
* Store
* Organize
* Analyze*

* **Query:** A request for data or information from a database.

Suggested order in which you write your SQL queries:

```sql
SELECT \[choose the column(s) you want]_
FROM \[from the appropriate table]_
WHERE \[a certain condition is met]_
```
Another example:
```sql
WHERE field1 LIKE 'Ch%'
```

You can conclude that the LIKE clause is very powerful because it allows you to tell the database to look for a certain pattern! The percent sign % is used as a wildcard to match one or more characters. In the example above, both **Chavez** and **Chen** would be returned. Note that in some databases an asterisk * is used as the wildcard instead of a percent sign %.

## Comments

Some tables aren’t designed with descriptive enough naming conventions. In the example, field1 was the column for a customer’s last name, but you wouldn’t know it by the name. A better name would have been something such as last_name. In these cases, you can place comments alongside your SQL to help you remember what the name represents. Comments are text placed between certain characters, /* and */, or after two dashes --) as shown below.

```sql
SELECT

    field1 /* this is the last name column */

FROM

    table -- this is the customer data table  

WHERE

    field1 LIKE 'Ch%';
```

## Aliases

You can also make it easier on yourself by assigning a new name or **alias** to the column or table names to make them easier to work with (and avoid the need for comments). This is done with a SQL AS clause. In the example below, aliases are used for both a table name and a column. Within the database, the table is called actual_table_name and the column in that table is called actual_column_name. They are aliased as my_table_alias and my_column_alias, respectively. These aliases are good for the duration of the query only. An alias doesn’t change the actual name of a column or table in the database.

```sql
SELECT 

    my_table_alias.actual_column_name AS my_column_alias

FROM

    actual_table_name AS my_table_alias
```
<> means "does not equal". Example:
```sql
SELECT
    *
FROM
    Employee
WHERE
    jobCode <> 'INT' 
      AND salary <= 30000;
```

Continue in [[Module 4 - Become a fair and impactful data professional]]
