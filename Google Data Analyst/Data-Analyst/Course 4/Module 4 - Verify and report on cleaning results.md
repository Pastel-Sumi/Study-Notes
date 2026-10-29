* **Verification:** A process to confirm that a data-cleaning effort was well-executed and the resulting data is accurate and reliable
* **Changelog:** A file containing a chronologically ordered list of modifications made to a project.

See the big picture when verifying data-cleaning
1. Consider the business problem.
2. Consider the goal.
3. Consider the data.

## Correct the most common problems

Make sure you identified the most common problems and corrected them, including:

- **Sources of errors**: Did you use the right tools and functions to find the source of the errors in your dataset?
- **Null data**: Did you search for NULLs using conditional formatting and filters?
- **Misspelled words**: Did you locate all misspellings?
- **Mistyped numbers**: Did you double-check that your numeric data has been entered correctly?
- **Extra spaces and characters**: Did you remove any extra spaces or characters using the **TRIM** function?
- **Duplicates**: Did you remove duplicates in spreadsheets using the **Remove Duplicates** function or **DISTINCT** in SQL?
- **Mismatched data types**: Did you check that numeric, date, and string data are typecast correctly?
- **Messy (inconsistent) strings**: Did you make sure that all of your strings are consistent and meaningful?
- **Messy (inconsistent) date formats**: Did you format the dates consistently throughout your dataset?
- **Misleading variable labels (columns)**: Did you name your columns meaningfully?
- **Truncated data:** Did you check for truncated or missing data that needs correction?
- **Business Logic**: Did you check that the data makes sense given your knowledge of the business?

![[Pasted image 20260609212050.png]]

* **Documentation:** The process of tracking changes, additions, deletions, and errors involved in your data-cleaning effort.

![[Pasted image 20260609214203.png]]

### Other terms
**CASE:** A SQL statement that returns records that meet conditions by including an if/then statement in a query

**Changelog:** A file containing a chronologically ordered list of modifications made to a project

**COUNTA:** A spreadsheet function that counts the total number of values within a specified range

**Find and replace:** A tool that finds a specified search term and replaces it with something else

**Verification:** A process to confirm that a data-cleaning effort was well executed and the resulting data is accurate and reliable