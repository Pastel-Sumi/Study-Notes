* **Dirty data:** Data that is incomplete, incorrect or irrelevant to the problem you're trying to solve.
* **Clean data:** Data that is complete, correct and relevant to the problem you're trying to solve.
* **Data engineers:** Transform data into a useful format for analysis and give it a reliable infrastructure.
* **Data warehousing specialists:** Develop processes and procedures to effectively store and organize data.
* **Null:** An indication that a value does not exist in a dataset.

![[Pasted image 20260605233738.png]]
### **Duplicate data**

|Description|Possible causes|Potential harm to businesses|
|---|---|---|
|Any data record that shows up more than once|Manual data entry, batch data imports, or data migration|Skewed metrics or analyses, inflated or inaccurate counts or predictions, or confusion during data retrieval|

### **Outdated data**

|Description|Possible causes|Potential harm to businesses|
|---|---|---|
|Any data that is old which should be replaced with newer and more accurate information|People changing roles or companies, or software and systems becoming obsolete|Inaccurate insights, decision-making, and analytics|

### **Incomplete data**

|Description|Possible causes|Potential harm to businesses|
|---|---|---|
|Any data that is missing important fields|Improper data collection or incorrect data entry|Decreased productivity, inaccurate insights, or inability to complete essential services|

### **Incorrect/inaccurate data**

|Description|Possible causes|Potential harm to businesses|
|---|---|---|
|Any data that is complete but inaccurate|Human error inserted during data input, fake information, or mock data|Inaccurate insights or decision-making based on bad information resulting in revenue loss|

### **Inconsistent data**

|Description|Possible causes|Potential harm to businesses|
|---|---|---|
|Any data that uses different formats to represent the same thing|Data stored incorrectly or errors inserted during data transfer|Contradictory data points leading to confusion or inability to classify or segment customers|

* **Field length:** A tool for determining how many characters can be keyed into a field.
* **Data validation:** A tool for checking the accuracy and quality of data before adding or importing it.

## First steps towards clean data
* Fixing misspellings.
* Inconsistent capitalization.
* Incorrect punctuation and other typos.

* **Merger:** An agreement that unites two organizations into a single new one.
* **Data merging:** The process of combining two or more datasets into a single dataset.
* **Compatibility:** How well two or more datasets are able to work together.
	* Do I have all the data I need?
	* Does the data I need exist within these datasets?
	* Does the data need to be cleaned, or are they ready for me to user?
	* Are the datasets cleaned to the same standard?

![[Pasted image 20260606125825.png|697]]


- **Not checking for spelling errors**: Misspellings can be as simple as typing or input errors. Most of the time the wrong spelling or common grammatical errors can be detected, but it gets harder with things like names or addresses. For example, if you are working with a spreadsheet table of customer data, you might come across a customer named “John” whose name has been input incorrectly as “Jon” in some places. The spreadsheet’s spellcheck probably won’t flag this, so if you don’t double-check for spelling errors and catch this, your analysis will have mistakes in it. 
    
- **Forgetting to document errors**: Documenting your errors can be a big time saver, as it helps you avoid those errors in the future by showing you how you resolved them. For example, you might find an error in a formula in your spreadsheet. You discover that some of the dates in one of your columns haven’t been formatted correctly. If you make a note of this fix, you can reference it the next time your formula is broken, and get a head start on troubleshooting. Documenting your errors also helps you keep track of changes in your work, so that you can backtrack if a fix didn’t work. 
    
- **Not checking for misfielded values**: A misfielded value happens when the values are entered into the wrong field. These values might still be formatted correctly, which makes them harder to catch if you aren’t careful. For example, you might have a dataset with columns for cities and countries. These are the same type of data, so they are easy to mix up. But if you were trying to find all of the instances of Spain in the country column, and Spain had mistakenly been entered into the city column, you would miss key data points. Making sure your data has been entered correctly is key to accurate, complete analysis. 
    
- **Overlooking missing values**: Missing values in your dataset can create errors and give you inaccurate conclusions. For example, if you were trying to get the total number of sales from the last three months, but a week of transactions were missing, your calculations would be inaccurate.  As a best practice, try to keep your data as clean as possible by maintaining completeness and consistency.
    
- **Only looking at a subset of the data**: It is important to think about all of the relevant data when you are cleaning. This helps make sure you understand the whole story the data is telling, and that you are paying attention to all possible errors. For example, if you are working with data about bird migration patterns from different sources, but you only clean one source, you might not realize that some of the data is being repeated. This will cause problems in your analysis later on. If you want to avoid common errors like duplicates, each field of your data requires equal attention.
    
- **Losing track of business objectives**: When you are cleaning data, you might make new and interesting discoveries about your dataset-- but you don’t want those discoveries to distract you from the task at hand. For example, if you were working with weather data to find the average number of rainy days in your city, you might notice some interesting patterns about snowfall, too. That is really interesting, but it isn’t related to the question you are trying to answer right now. Being curious is great! But try not to let it distract you from the task at hand.  
    
- **Not fixing the source of the error:** Fixing the error itself is important. But if that error is actually part of a bigger problem, you need to find the source of the issue. Otherwise, you will have to keep fixing that same error over and over again. For example, imagine you have a team spreadsheet that tracks everyone’s progress. The table keeps breaking because different people are entering different values. You can keep fixing all of these problems one by one, or you can set up your table to streamline data entry so everyone is on the same page. Addressing the source of the errors in your data will save you a lot of time in the long run. 
    
- **Not analyzing the system prior to data cleaning:** If we want to clean our data and avoid future errors, we need to understand the root cause of your dirty data. Imagine you are an auto mechanic. You would find the cause of the problem before you started fixing the car, right? The same goes for data. First, you figure out where the errors come from. Maybe it is from a data entry error, not setting up a spell check, lack of formats, or from duplicates. Then, once you understand where bad data comes from, you can control it and keep your data clean.
    
- **Not backing up your data prior to data cleaning**: It is always good to be proactive and create your data backup before you start your data clean-up. If your program crashes, or if your changes cause a problem in your dataset, you can always go back to the saved version and restore it. The simple procedure of backing up your data can save you hours of work-- and most importantly, a headache. 
    
- **Not accounting for data cleaning in your deadlines/process**: All good things take time, and that includes data cleaning. It is important to keep that in mind when going through your process and looking at your deadlines. When you set aside time for data cleaning, it helps you get a more accurate estimate for ETAs for stakeholders, and can help you know when to request an adjusted ETA.

* **Conditional formatting:** A spreadsheet tool that changes how cells appear when values meet specific conditions
* **Remove duplicates:** A tool that automatically searches for and eliminates duplicate entries from a spreadsheet.
* **Text string:** A group of characters within a cell, most often composed of letters.
* **Split:** A tool that divides text around a specified character and puts each fragment into a new, separate cell.
* **Concatenate:** A function that joins multiple text strings into a single string.
* **Trim:** A function that removes leading, trailing, and repeated spaces in data.
* LEFT, RIGHT, MID to get substrings from a string.

|**Task**|**Can it be automated?**|**Why?**|
|---|---|---|
|Communicating with your team and stakeholders|No|Communication is key to understanding the needs of your team and stakeholders as you complete the tasks you are working on. There is no replacement for person-to-person communications.|
|Presenting your findings|No|Presenting your data is a big part of your job as a data analyst. Making data accessible and understandable to stakeholders and creating data visualizations can’t be automated for the same reasons that communications can’t be automated.|
|Preparing and cleaning data|Partially|Some tasks in data preparation and cleaning can be automated by setting up specific processes, like using a programming script to automatically detect missing values.|
|Data exploration|Partially|Sometimes the best way to understand data is to see it. Luckily, there are plenty of tools available that can help automate the process of visualizing data. These tools can speed up the process of visualizing and understanding the data, but the exploration itself still needs to be done by a data analyst.|
|Modeling the data|Yes|Data modeling is a difficult process that involves lots of different factors; luckily there are tools that can completely automate the different stages.|

### **Your cleaning checklist**

Start developing your personal approach to cleaning data by creating a checklist to help you identify problems in your data efficiently and identify the scale and scope of your dataset. Think of this checklist as your default “what to search for” list.

Here are some examples of common data cleaning tasks you could include in your checklist:

- **Determine the size of the dataset:** Large datasets may have more data quality issues and take longer to process. This may impact your choice of data cleaning techniques and how much time to allocate to the project.
    
- **Determine the number of categories or labels:** By understanding the number and nature of categories and labels in a dataset, you can better understand the diversity of the dataset. This understanding also helps inform data merging and migration strategies.
    
- **Identify missing data:** Recognizing missing data helps you understand data quality so you can take appropriate steps to remediate the problem. Data integrity is important for accurate and unbiased analysis.
    
- **Identify unformatted data:** Identifying improperly or inconsistently formatted data helps analysts ensure data uniformity. This is essential for accurate analysis and visualization.
    
- **Explore the different data types:** Understanding the types of data in your dataset (for instance, numerical, categorical, text) helps you select appropriate cleaning methods and apply relevant data analysis techniques.

# Terms for this module
**Clean data:** Data that is complete, correct, and relevant to the problem being solved

**Compatibility:** How well two or more datasets are able to work together

**CONCATENATE:** A spreadsheet function that joins together two or more text strings

**Conditional formatting:** A spreadsheet tool that changes how cells appear when values meet specific conditions

**Data engineer:** A professional who transforms data into a useful format for analysis and gives it a reliable infrastructure

**Data mapping:** The process of matching fields from one data source to another

**Data merging:** The process of combining two or more datasets into a single dataset

**Data validation:** A tool for checking the accuracy and quality of data

**Data warehousing specialist:** A professional who develops processes and procedures to effectively store and organize data

**Delimiter:** A character that indicates the beginning or end of a data item

**Dirty data:** Data that is incomplete, incorrect, or irrelevant to the problem to be solved

**Duplicate data:** Any record that inadvertently shares data with another record

**Field length:** A tool for determining how many characters can be keyed into a spreadsheet field

**Incomplete data:** Data that is missing important fields

**Inconsistent data:** Data that uses different formats to represent the same thing

**Incorrect/inaccurate data:** Data that is complete but inaccurate

**LEFT:** A function that returns a set number of characters from the left side of a text string 

**LEN:** A function that returns the length of a text string by counting the number of characters it contains

**Length:** The number of characters in a text string

**Merger:** An agreement that unites two organizations into a single new one

**MID:** A function that returns a segment from the middle of a text string

**Null:** An indication that a value does not exist in a dataset

**Outdated data:** Any data that has been superseded by newer and more accurate information

**Remove duplicates:** A spreadsheet tool that automatically searches for and eliminates duplicate entries from a spreadsheet

**Split:** A function that divides text around a specified character and puts each fragment into a new, separate cell

**Substring:** A smaller subset of a text string

**Text string:** A group of characters within a cell, most often composed of letters

**TRIM:** A function that removes leading, trailing, and repeated spaces in data

**Unique:** A value that can’t have a duplicate

Continue in [[Module 3 - Data cleaning with SQL]]
