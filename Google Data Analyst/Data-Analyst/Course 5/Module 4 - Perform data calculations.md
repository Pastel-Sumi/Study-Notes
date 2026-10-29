* **Conditional formatting:** A spreadsheet tool that changes how cells appear when values meet specific conditions.
* **Summary table:** A table used to summarize statistical information about data.
* **SUMIF:** A function that adds numeric data based on one condition.
* **SUMPRODUCT:** A function that multiplies arrays and returns the sum of those products.
* **Array:** A collection of values in cells.
* **Pivot table:** Let you view data in multiple ways to find insights and trends.
* **Calculated field:** A new field within a pivot table that carries out certain calculations based on the values of other fields.
* **Operator:** A symbol that names the type of operation or calculation to be performed in a formula.
* **GROUP BY:** A command that groups rows that have the same values from a table into summary rows.
* **Extract command:** Lets us pull one part of a given date to use.
* **Data validation process:** Checking and rechecking the quality of your data so that it is complete, accurate, secure and consistent.
* **Data security:** Protecting data from unauthorized access or corruption by adopting safety measures.
* **Profit Margin:** A percentage that indicates how many cents of profit has been generated for each dollar of sale.

## Types of data validation
![[Pasted image 20260706215630.png]]
* **Purpose**: Check that the data matches the data type defined for a field.
-  **Example**: Data values for school grades 1-12 must be a numeric data type.
- **Limitations**: The data value 13 would pass the data type validation but would be an unacceptable value. For this case, data range validation is also needed.
 
![[Pasted image 20260706215725.png|697]]
* **Purpose**: Check that the data falls within an acceptable range of values defined for the field.
- **Example**: Data values for school grades should be values between 1 and 12.
- **Limitations**: The data value 11.5 would be in the data range and would also pass as a numeric data type. But, it would be unacceptable because there aren't half grades. For this case, data constraint validation is also needed.

![Icon with gears and the words data constraints](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/DUa8GZEkTR6GvBmRJC0emw_a9e6271e8f1c4cb0820ec3d6ee34f4eb_Screen-Shot-2021-02-08-at-5.27.40-PM.png?expiry=1783475745662&hmac=oomVYLf4Agz4ZAhwDvwW-K9NZpIYea7QhRNc6itBDrs)

- **Purpose**: Check that the data meets certain conditions or criteria for a field. This includes the type of data entered as well as other attributes of the field, such as number of characters.
- **Example**: Content constraint: Data values for school grades 1-12 must be whole numbers.
- **Limitations**: The data value 13 is a whole number and would pass the content constraint validation. But, it would be unacceptable since 13 isn’t a recognized school grade. For this case, data range validation is also needed.

![Icon of a traffic light with words data consistency](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Xlu9FFgIRDGbvRRYCFQx-w_6eaa5307239541e9a5e0c77a343f9c8b_Screen-Shot-2021-02-08-at-5.30.56-PM.png?expiry=1783475745662&hmac=AkL0Lp-cu4-VqKok05IAwDZm2WF322prG9a2_bm0KWM)

- **Purpose**: Check that the data makes sense in the context of other related data.
- **Example**: Data values for product shipping dates can’t be earlier than product production dates.
- **Limitations**: Data might be consistent but still incorrect or inaccurate. A shipping date could be later than a production date and still be wrong.    

![Icon of a clipboard checklist with words Data structure](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/6kdSdq1vQfeHUnatbwH3Lg_02d9444056b340e58377aa792ecb0d43_Screen-Shot-2021-02-08-at-5.33.03-PM.png?expiry=1783475745662&hmac=ww2dSiwgsUiMteK5x6H-pqFaEscqJ2-bWwhmxchFXhc)

- **Purpose**: Check that the data follows or conforms to a set structure.
- **Example**: Web pages must follow a prescribed structure to be displayed properly.
- **Limitations**: A data structure might be correct with the data still incorrect or inaccurate. Content on a web page could be displayed properly and still contain the wrong information.

![Icon with computer arrows traveling to multiple users with the word Code validation](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Saof9D7aT8eqH_Q-2k_Hyg_d144822d70ac4ec3b22b5126c0b32e60_Screen-Shot-2021-02-08-at-5.34.42-PM.png?expiry=1783475745662&hmac=5R5KBuGp8a2KzRx5Wj8NcpPnSNeQuwP2hpW9j9uoGiE)

- **Purpose:** Check that the application code systematically performs any of the previously mentioned validations during user data input.
- **Example:** Common problems discovered during code validation include: more than one data type allowed, data range checking not done, or ending of text strings not well defined.
- **Limitations:** Code validation might not validate all possible variations with data input.


* **Temporary table:** A database table that is created and exists temporarily on a database server. Deleted automatically when you end your SQL session.
	* The WITH clause is a type of temporary table that you can query from multiple times. (In BigQuery).
```sql
WITH
	new_table_data AS (
	SELECT *
	FROM
	Existing_table
	WHERE
	Tripduration >=60
	)
```
	
* SELECT INTO statements also create temporary tables.	
```sql
SELECT *
INTO
AfricaSales
FROM
GlobalSales
WHERE
Region = "Africa"
```
* CREATE TABLE statements also create a table (that gets added to the database).
Temporary table creation in other databases:

Continues in [[Course 6 - Share Data Through the Art of Visualization]]
