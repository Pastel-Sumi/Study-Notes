Data validation:
* Add dropdown lists with predetermined options
* Create custom checkboxes
* Protect structured data and formulas.

|Starting with|CAST function can convert to:|
|---|---|
|Numeric (number)|- Integer - Numeric (number) - Big number - Floating integer - String|
|String|- Boolean - Integer - Numeric (number) - Big number - Floating integer - String - Bytes - Date - Date time - Time - Timestamp|
|Date|- String - Date - Date time - Timestamp|
```SQL
SELECT CAST(MyCount AS STRING) FROM MyTable
```

## The SAFE_CAST function

Using the CAST function in a query that fails returns an error in BigQuery. To avoid errors in the event of a failed query, use the SAFE_CAST function instead. The SAFE_CAST function returns a value of Null instead of an error when a query fails. 

The syntax for SAFE_CAST is the same as for CAST. Simply substitute the function directly in your queries. The following SAFE_CAST statement returns a string from a date.

```sql
SELECT SAFE_CAST(MyDate AS STRING) FROM MyTable
```
### **Combine data in spreadsheets**

In spreadsheets, you use the CONCATENATE function to join together two or more text strings, such as combining street addresses and primary contacts in a business’ vendor database.

The basic syntax is =CONCATENATE(item 1, item 2). You can add multiple items by separating them with commas. Where appropriate, such as when you’re combining a customer’s first and last name, you should add a space between the items you’re combining by typing quotation marks space quotation marks [“ ”] between the items. Separate this information by a comma as well. This would change the formula to: =CONCATENATE(item 1, " ", item 2).

### **Combine data in SQL**

In SQL, use the CONCAT function to join strings together to create new text strings. You might combine data simply to improve the readability of reports (such as combining a customer’s first and last name when generating a customer list). Or, you might combine data to generate a unique identifier for the rows in a table. Here is the basic syntax:
```sql
SELECT CONCAT(field1, " ", field2)
FROM [table_name]
```

### CONCAT_WS

Now, you're tasked with creating a report that includes a website's URL components: the protocol (http), domain name (your_company), and domain (com). You'd use CONCAT_WS, which stands for CONCAT With Separator, to achieve this. It's similar to CONCAT, but it includes a separator, such as a space or period, between the strings.

```sql
SELECT CONCAT_WS('.', 'www', 'your_company', 'com') AS website FROM web_data;
```

### CONCAT **with** ||

In BigQuery, you can use the || operator to concatenate strings. For instance, if you're working with a dataset of book information and want to create a full title by combining the book's name and its edition, you could use ||, like so:

```sql
SELECT book_name || ' - ' || edition AS full_book_title FROM library;
```
This script combines the book name and edition, separated by a hyphen for clarity, providing a complete, informative title for your records.

| **Function/ operator** | **Use**                                                                       | **Example**                              | **Result**     |
| ---------------------- | ----------------------------------------------------------------------------- | ---------------------------------------- | -------------- |
| CONCAT                 | Concatenate strings to create new text strings                                | CONCAT('Google', '.com')                 | Google.com     |
| CONCAT_WS              | Concatenate two or more strings together with a separator between each string | CONCAT_WS(' . ', 'www', 'google', 'com') | www.google.com |
| \|                     | Concatenate two or more strings together with the \| operator                 | 'Google' \| '.com'                       | Google.com     |

Continues in [[Module 3 - Aggregate data for analysis ]]
