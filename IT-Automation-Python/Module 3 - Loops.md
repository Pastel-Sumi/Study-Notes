* **while loops:** Instruct your computer to continuously execute your code based on the value of a condition.
* **Initializing:** To give an initial value to a variable.
* **Infinite loop:** A loop that keeps executing and never stops.
* **for loop:** Iterates over a sequence of values.

The **range()** function can take up to three parameters:  **range(start, stop, step)** 

**Start**  The first item in the **range()** function parameters is the starting position of the range. The default is the first index position, which points to the numeric value 0. This value is included in the range. 

**Stop** The second item in the **range()** function parameters is the ending position of the range. There is no default index position, so this index number must be given to the **range()** parameters. For example, the line **for n in range(4)** will loop 4 times with the **n** variable starting at 0 and looping 4 index positions: 0, 1, 2, 3. As you can see, **range(4)** (meaning index position 4) ends at the numeric value 3. In Python, this structure may be phrased as “the end-of-range value is _excluded_ from the range.” In order to include the value 4 in  **range(4)**, the syntax can be written as **range(4+1)** or **range(5)**. Both of these ranges will produce the numeric values 0, 1, 2, 3, 4.

**Step** The third item in the **range()** function parameters is the incremental step value. The default increment is +1. The default value can be overridden with any valid increment. However, note that the loop will still end at the end-of-range index position, regardless of the incremental value. For example, if you have a loop with the range: **for n in range(1, 5, 6)**, the range will only produce the numeric value 1. This is because the incremental value of 6 exceeded the ending point of the range.


## Recursion
* **Recursion:** The repeated application of the same procedure to a smaller problem.
"Recursion lets us tackle complex problems by reducing the problem to a simpler one".
"In programming, recursion is a way of doing a repetitive task by having a function call itself."
* The idea is to eventually reach the **base case** via the **recursive cases**.
The usual structure:
```python
def recursive_function(parameters):
    if base_case_condition(parameters):
        return base_case_value
    recursive_function(modified_parameters)
```

Continues in [[Module 4 - Strings, Lists and Dictionaries]]
