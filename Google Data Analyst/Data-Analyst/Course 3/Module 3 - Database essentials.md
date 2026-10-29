* **Database:** A collection of data stored in a computer system.
* **Metadata:** Data about data.
* **Relational database:** A database that contains a series of related tables that can be connected via their relationships.
* **Primary key:** An identifier that references a column in which each value is unique.
* **Foreign key:** A field within a table that is a primary key in another table.

## Relational databases

A **relational database** is a database that contains a series of tables that can be connected to form relationships. Basically, they allow data analysts to organize and link data based on what the data has in common. 
In a non-relational table, you will find all of the possible variables you might be interested in analyzing all grouped together. This can make it really hard to sort through. This is one reason why relational databases are so common in data analysis: they simplify a lot of analysis processes and make data easier to find and use across an entire database. 
**Normalization** is a process of organizing data in a relational database. For example, creating tables and establishing relationships between those tables. It is applied to eliminate data redundancy, increase data integrity, and reduce complexity in a database.

![[Pasted image 20260602123359.png]]

* **Descriptive metadata:** Metadata that describes a piece of data and can be used to identify it at a later point in time (ISBN in a book).
* **Structural metadata:** Metadata that indicates how a piece of data is organized and whether it is a part of one, or more than one, data collection (Pages of a book forming a chapter).
* **Administrative metadata:** Metadata that indicates the technical source of a digital asset (metadata of a picture).

## Elements of metadata

Before examining metadata examples, it’s important to understand what type of information metadata typically provides:

- **File or document type:** What type of file or document are you examining?
    
- **Date, time, and creator:** When was it created? Who created it? When was it last modified?
    
- **Title and description:** What is the name of the item you are examining? What type of content does it contain?
    
- **Geolocation:** If you’re examining a photo, where was it taken?
    
- **Tags and categories:** What is the general overview of the item that you have? Is it indexed or described in a specific way?
    
- **Who last modified it and when:** Were any changes made to the file? If yes, when were the most recent modifications made?
    
- **Who can access or update it:** If you’re examining a dataset, is it public? Are special permissions needed to customize or modify it?

"Metadata is stored in a single, central location, and gives the company standardized information about all of its data".

* **Data governance:** A process to ensure the formal management of a company's data assets.


### Access different data sources
* **CSV:** Comma-separated values. Saves data in a table format.

### **The** IMPORTRANGE **function**

In Google Sheets, the IMPORTRANGE function can import all or part of a dataset from another Google Sheet.

To use this function, you need two pieces of information:

1. The URL of the Google Sheet from which you’ll import data.
    
2. The name of the sheet and the range of cells you want to import into your Google Sheet.
    

Once you have this information, open the Google Sheet into which you want to import data and select the cell into which the first cell of data should be copied. Enter = to indicate you will enter a function, then complete the IMPORTRANGE function with the URL and range you identified in the following manner: `=IMPORTRANGE("URL", "sheet_name!cell_range")`. Note that an exclamation point separates the sheet name and the cell range in the second part of this function.
Ex: `=IMPORTRANGE("https://docs.google.com/thisisatestabc123", "sheet1!A1:F13")`

### **The** IMPORTHTML **function**

Importing HTML tables is a basic method to extract data from public web pages. This process is often called “scraping.”

### Sort and filter data
* **Sorting data:** Arranging data into a meaningful order to make it easier to understand, analyze, and visualize.
* **Filtering:** Showing only the data that meets a specific criteria while hiding the rest.

### Large datasets in SQL
Big query stuff.

### Other terms
**Administrative metadata:** Metadata that indicates the technical source of a digital asset

**CSV (comma-separated values) file:** A delimited text file that uses a comma to separate values

**Data governance:** A process for ensuring the formal management of a company’s data assets

**Descriptive metadata:** Metadata that describes a piece of data and can be used to identify it at a later point in time

**Foreign key:** A field within a database table that is a primary key in another table (Refer to primary key)

**FROM:** The section of a query that indicates where the selected data comes from

**Geolocation:** The geographical location of a person or device by means of digital information

**Metadata:** Data about data

**Metadata repository:** A database created to store metadata

**Naming conventions:** Consistent guidelines that describe the content, creation date, and version of a file in its name

**Normalized database:** A database in which only related data is stored in each table

**Notebook:** An interactive, editable programming environment for creating data reports and showcasing data skills

**Primary key:** An identifier in a database that references a column in which each value is unique (Refer to foreign key)

**Redundancy:** When the same piece of data is stored in two or more places

**Schema:** A way of describing how something, such as data, is organized

**SELECT:** The section of a query that indicates the subset of a dataset

**Structural metadata:** Metadata that indicates how a piece of data is organized and whether it is part of one or more than one data collection

**WHERE:** The section of a query that specifies criteria that the requested data must meet

**World Health Organization:** An organization whose primary role is to direct and coordinate international health within the United Nations system

Continue in [[Module 4 - Organize and protect data]]