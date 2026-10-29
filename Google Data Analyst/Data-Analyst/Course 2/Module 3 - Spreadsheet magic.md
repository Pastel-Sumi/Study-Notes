Spreadsheet tasks:
* Organize your data.
	* Pivot table.
		* Sort and filter.
* Calculate your data.
	* Formulas.
	* Functions.

## Spreadsheets and the data life cycle
![[Pasted image 20260524205946.png]] * **Plan** for the users who will work within a spreadsheet by developing organizational standards. This can mean formatting your cells, the headings you choose to highlight, the color scheme, and the way you order your data points. When you take the time to set these standards, you will improve communication, ensure consistency, and help people be more efficient with their time.
    
- **Capture** data by the source by connecting spreadsheets to other data sources, such as an online survey application or a database. This data will automatically be updated in the spreadsheet. That way, the information is always as current and accurate as possible.
    
- **Manage** different kinds of data with a spreadsheet. This can involve storing, organizing, filtering, and updating information. Spreadsheets also let you decide who can access the data, how the information is shared, and how to keep your data safe and secure. 
    
- **Analyze** data in a spreadsheet to help make better decisions. Some of the most common spreadsheet analysis tools include formulas to aggregate data or create reports, and pivot tables for clear, easy-to-understand visuals. 
    
- **Archive** any spreadsheet that you don’t use often, but might need to reference later with built-in tools. This is especially useful if you want to store historical data before it gets updated. 
    
- **Destroy** your spreadsheet when you are certain that you will never need it again, if you have better backup copies, or for legal or security reasons. Keep in mind, lots of businesses are required to follow certain rules or have measures in place to make sure data is destroyed properly.

* **Operator:** A symbol that names the type of operation or calculation to be performed.
* **Cell reference:** A cell or a range of cells in a worksheet that can be used in a formula.
* **Range:** A collection of two or more cells.
* **"#DIV/0!"**: A formula is trying to divide a value in a cell by 0 or by an empty cell.
* **"#N/A":** Data in a formula can't be found by the spreadsheet.

|Error|Description|Example|
|---|---|---|
|**#DIV/0!**|A formula is trying to divide a value in a cell by 0 (or an empty cell with no value)|=B2/B3, when the cell B3 contains the value 0|
|**#ERROR!**|(Google Sheets only)  Something can’t be interpreted as it has been input. This is also known as a parsing error.|=COUNT(B1:D1 C1:C10) is invalid because the cell ranges aren't separated by a comma|
|**#N/A**|A formula can't find the data|The cell being referenced can't be found|
|**#NAME?**|The name of a formula or function used isn't recognized|The name of a function is misspelled|
|**#NUM!**|The spreadsheet can't perform a formula calculation because a cell has an invalid numeric value|=DATEDIF(A4, B4, "M") is unable to calculate the number of months between two dates because the date in cell A4 falls after the date in cell B4|
|**#REF!**|A formula is referencing a cell that isn't valid|A cell used in a formula was in a column that was deleted|
|**#VALUE!**|A general error indicating a problem with a formula or with referenced cells|There could be problems with spaces or text, or with referenced cells in a formula; you may have additional work to find the source of the problem.|
### **Difference between formulas and functions**

- A formula is a set of instructions used to perform a calculation using the data in a spreadsheet.
    
- A function is a preset command that automatically performs a specific process or task using the data in a spreadsheet.

### **Relative, absolute, and mixed references**

- Relative references (cells referenced without a dollar sign, like **A2**) will change when you copy and paste the function into a different cell. With relative references, the location of the cell that contains the function determines the cells used by the function.
    
- Absolute references (cells fully referenced with a dollar sign, like **$A$2**) will not change when you copy and paste the function into a different cell. With absolute references, the cells referenced always remain the same.
    
- Mixed references (cells partially referenced with a dollar sign, like **$A2** or **A$2**) will change when you copy and paste the function into a different cell. With mixed references, the location of the cell that contains the function determines the cells used by the function, but only the row or column is relative (not both).
    
- In spreadsheets, you can press the **F4** key to toggle between relative, absolute, and mixed references in a function. Click the cell containing the function, highlight the referenced cells in the formula bar, and then press **F4** to toggle between and select relative, absolute, or mixed referencing.

### **Data ranges**

- When you click a cell that contains a function, colored data ranges in the formula bar indicate which cells are being used in the spreadsheet. There are different colors for each unique range in a function.
    
- Colored data ranges help prevent you from getting lost in complex functions.
    
- In spreadsheets, you can press the **F2** key to highlight the range of data used by a function. Click the cell containing the function, highlight the range of data used by the function in the formula bar, and then press **F2**. The spreadsheet will go to and highlight the cells specified by the range.

### Save time with structured thinking
* **Problem domain:** The specific area of analysis that encompasses every activity affecting or affected by the problem.
* **Structured thinking:** The process of recognizing the current problem or situation, organizing available information, revealing gaps and opportunities, and identifying the options.
* **Scope of work(SOW):** An agreed-upon outline of the work you're going to perform on a project. Sets the expectations and boundaries. It may be included in a statement of work to help define project outcomes.
* **Statement of work:** A statement of work is a document that clearly identifies the products and services a vendor or contractor will provide to an organization. It includes objectives, guidelines, deliverables, schedule, and costs.


### What is a good SOW?
- **Deliverables**: What work is being done, and what things are being created as a result of this project? When the project is complete, what are you expected to deliver to the stakeholders? Be specific here. Will you collect data for this project? How much, or for how long?
	- Avoid vague statements. For example, “fixing traffic problems” doesn’t specify the scope. This could mean anything from filling in a few potholes to building a new overpass. Be specific! Use numbers and aim for hard, measurable goals and objectives. For example: “Identify top 10 issues with traffic patterns within the city limits, and identify the top 3 solutions that are most cost-effective for reducing traffic congestion.”
- **Milestones**: This is closely related to your timeline. What are the major milestones for progress in your project? How do you know when a given part of the project is considered complete?
	- Milestones can be identified by you, by stakeholders, or by other team members such as the Project Manager. Smaller examples might include incremental steps in a larger project like “Collect and process 50% of required data (100 survey responses)”, but may also be larger examples like ”complete initial data analysis report” or “deliver completed dashboard visualizations and analysis reports to stakeholders”.
- **Timeline**: Your timeline will be closely tied to the milestones you create for your project. The timeline is a way of mapping expectations for how long each step of the process should take. The timeline should be specific enough to help all involved decide if a project is on schedule. When will the deliverables be completed? How long do you expect the project will take to complete? If all goes as planned, how long do you expect each component of the project will take? When can we expect to reach each milestone?
- **Reports**: Good SOWs also set boundaries for how and when you’ll give status updates to stakeholders. How will you communicate progress with stakeholders and sponsors, and how often? Will progress be reported weekly? Monthly? When milestones are completed? What information will status reports contain?
At a minimum, any SOW should answer all the relevant questions in the above areas. Note that these areas may differ depending on the project. But at their core, the SOW document should always serve the same purpose by containing information that is specific, relevant, and accurate. If something changes in the project, your SOW should reflect those changes.

### The importance of context
* **Context:** The condition in which something exists or happens.
**Context can turn raw data into meaningful information.** It is very important for data analysts to contextualize their data. This means giving the data perspective by defining it. To do this, you need to identify:

- Who: The person or organization that created, collected, and/or funded the data collection
- What: The things in the world that data could have an impact on
- Where: The origin of the data
- When: The time when the data was created or collected
- Why: The motivation behind the creation or collection
- How: The method used to create or collect it

### Other terms
* **Open data:** Data that is available to the public.
* **Revenue:** The total amount of income generated by the sale of goods or services.
* **Sorting:** The process of arranging data into a meaningful order to make it easier to understand, analyze, and visualize.


Continue in [[Module 4 - Always remember the stakeholder]]
