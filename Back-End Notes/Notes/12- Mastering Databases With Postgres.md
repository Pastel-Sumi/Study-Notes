## I. Introduction to Databases ([0:00](https://www.youtube.com/watch?v=F7Vwp2Xo5Do) - [9:54](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=594s)) 
* **Persistence**: The ability of a program to keep information stored so it survives even after the program stops running, such as saving tasks in a to-do list app. 
* **Database**: A system for storing, creating, reading, updating, and deleting (**CRUD**) data. While basic storage like text files or browser local storage act as databases, professional backend systems primarily use **disk-based databases**. 
* **Disk-based Storage**: Uses *HDD or SSD because it is cheaper and offers more capacity than *RAM* (main memory), which is faster but more expensive and limited in supply. 
* **DBMS (Database Management System)**: Software that handles the organization, access, integrity (data accuracy/validity), and security of data, replacing inefficient manual management via text files. 
## II. Why DBMS over Text Files? ([12:32](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=752s) - [18:29](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=1109s)) 
* **Parsing Issues**: Manually reading/splitting text files is slow and error-prone, especially for complex or large data. 
* **Lack of Structure**: Text files are fluid and do not enforce consistent data formats (e.g., ensuring a payment field only contains numbers). 
* **Concurrency**: DBMS systems handle multiple users modifying the same data simultaneously without causing errors or inconsistent results. 
## III. Relational Databases and Postgres ([18:29](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=1109s) - [31:04](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=1864s&pp=0gcJCTEAlc8ueATH)) 
* **Relational Databases**: Organize data into **tables, rows, and columns**. Relationships are defined using keys like **foreign keys**. 
* **Postgres**: Recommended as the first choice for most projects due to its rich feature set and strong **JSON** support. 
## IV. Data Types in Postgres ([33:15](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=1995s) - [53:23](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=3203s)) 
* **Serial**: An integer that automatically increments (e.g., 1, 2, 3) for primary keys. Use **Big Serial** for larger capacity. 
* **Numeric/Decimal**: Best for **price* or data where mathematical accuracy is critical.
* **Float/Real**: Faster to process; use when small discrepancies in accuracy are acceptable (e.g., scientific data).
* **String Types**: 
	* **Char**: Fixed-length; adds spaces if the input is shorter than defined. 
	* **Varchar**: Variable length; stores only the input length up to a defined limit. 
	* **Text**: The modern standard; handles any amount of text without arbitrary limits. 
* **Boolean**: Stores true/false values. 
* **Date/Time**: Includes `date`, `time`, `timestamp` (date + time), and `timestamptz` (includes time zone information). 
* **UUID**: A popular, unique identifier for primary keys. 
* **JSON/JSONB**: Native support; *JSONB* (Binary) is preferred for better performance and indexing.
## V. Migrations and Database Design ([54:19](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=3259s) - [1:18:21](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=4701s)) 
* **Migrations**: A system to track and apply structural changes to the database (e.g., adding tables) over time using versioned files. 
* **Up Migrations**: Apply changes (e.g., `CREATE TABLE`). 
* **Down Migrations**: Revert those changes. 
* **Enums**: Custom data types for columns with a predefined list of allowed values (e.g., status: active, completed, archived). This enforces data integrity. 
* **Naming Conventions**: Use plural table names (e.g., *users*) and small/snake case for fields to ensure case-insensitivity consistency in Postgres. 
## VI. Project Management Database Design ([1:18:21](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=4701s) - [1:39:18](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=5958s)) 
* **Users Table**: Stores core user data with a unique ID and email. 
* **User Profiles**: Linked to users via a **one-to-one relationship** using the user's ID as the primary key. This keeps personal bio/meta-data separate. 
* **Projects Table**: Stores project information and uses a **foreign key** to link an `owner_id` to a specific user. 
* **On Delete Restrict**: A safety constraint that prevents deleting a user if they are still an active owner of a project. 
* **Tasks Table**: Created with a **one-to-many relationship** to projects. 
* **Check Constraint**: Enforces data rules, such as limiting task priority values to between 1 and 5.
* **Project Members Table**: Uses a **many-to-many relationship** via a linking table. 
* **Composite Primary Key**: Combines `project_id` and `user_id` to ensure a user can only be added to a specific project once. 
* **On Delete Cascade**: If a project or user is deleted, their association in this table is automatically removed. 
## VII. Seeding and Data Retrieval ([1:40:24](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=6024s) - [1:59:52](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=7192s)) 
* **Seeding**: The process of inserting sample test data into tables to verify the database design works before moving to production. 
* **Joins**: 
	* **Left Join**: Used to fetch data from two tables (e.g., users and profiles) while ensuring that even if a user lacks a profile, their basic information is still returned. 
* **Parameterized Queries**: A vital security practice. Instead of inserting raw user input directly into a query, use placeholders to prevent malicious SQL injection attacks. 
## VIII. Advanced Querying and Optimization ([2:00:13](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=7213s) - [2:31:13](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=9073s)) 
* **Pagination**: Essential for list APIs. Using **OFFSET** and *LIMIT* ensures the system only returns a manageable chunk of data at a time rather than the entire database table. 
* **Indexing**: A technique to speed up data retrieval. Creating indexes on columns used frequently in **WHERE** clauses or join conditions allows the database to locate rows instantly instead of scanning the whole table. 
## IX. Triggers ([2:41:59](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=9719s) - [2:43:56](https://www.youtube.com/watch?v=F7Vwp2Xo5Do&t=9836s)) 
* **Functions & Triggers**: A custom function is created to set an `updated_at` timestamp. A trigger is then attached to tables to automatically run this function whenever a row is updated, ensuring the modification time is always accurate without manual input.