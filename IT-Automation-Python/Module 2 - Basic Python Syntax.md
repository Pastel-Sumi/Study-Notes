"Semantics is the meaning conveyed by the syntax."
* **String:** Known as a "data type".
* **Implicit conversion:** The interpreter automatically converts one data type into another.
* **Explicit conversion:** When code is written to manually convert one data type to another using a data type conversion function:
	* `str()` - Converts a value (often numeric) to a **string** data type
	* `int()` - Converts a value (usually a float) to an **integer** data type
	* `float()` - Converts a value (usually an integer) to a **float** data type
**Built-in functions** are functions that exist within Python and can be called directly.
The type() function returns the data type of its argument. The type() function helps you keep track of the data types of variables to avoid errors throughout your code.

|**Symbol**|**Name**|**Expression**|**Description**|
|---|---|---|---|
|**==**|Equality operator|a == b|a is equal to b|
|**!=**|Not equal to operator|a != b|a is **not** equal to b|
|**>**|Greater than operator|a > b|a is larger than b|
|**>=**|Greater than or equal to operator|a >= b|a is larger than or equal to b|
|**<**|Less than operator|a < b|a is smaller than b|
|**<=**|Less than or equal to operator|a <= b|a is smaller than or equal to b|

|**Expression**|**Description**|
|---|---|
|"a" **==** "a"|If string "a" is identical to string "a", returns True. Else, returns False|
|"a" **!=** "b"|If string "a" is **not** identical to string "b"|
|"a" **>** "b"|If string "a" has a larger Unicode value than string "b"|
|"a" **>=** "b"|If the Unicode value for string "a" is greater than or equal to the Unicode value of string "b"|
|"a" **<** "b"|If string "a"  has a smaller Unicode value than string "b"|
|"a" **<=** "b"|If the Unicode value for string "a" is smaller than or equal to the Unicode value of string "b"|

|**Expression**|**Description**|
|---|---|
|a **==** a **and** a **!=** b|True if both sides are True, otherwise False.|
|a **>** b **or** a **<=** c|True if either side is True. False if both sides are False.|
|**not** a **==** b|True if the statement is False, False if the statement is True.|
* **Branching:** The ability of a program to alter its execution sequence.

## **Terms and definitions from Course 1, Module 2**

**Built-in functions:** Functions that exist within Python and can be called directly

**Comments:** Notes to yourself and/or other programmers to make the purpose of the code clear

**Data types:** Classes of data (e.g., string, int, float, Boolean, etc.), which include the properties and behaviors of instances of the data type (variables)

**Explicit conversion:** This occurs when code is written to manually convert one data type to another using a data type conversion function

**Expression:** A combination of numbers, symbols, or other values that produce a result when evaluated

**Implicit conversion:** This occurs when the Python interpreter automatically converts one data type to another

**Logical operators:** Operators used to combine or manipulate boolean values (True or False) to create complex conditions for decision-making. 

**Parameter (argument):** A value passed into a function for use within the function, controlling the behavior of the CSV reader and writer

**Refactoring:** When a code is updated to be more self-documenting and clarify the intent 

**Return value**: This is the value or variable returned as the end result of a function

Continues in [[Module 3 - Loops]]
