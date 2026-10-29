## What is a Data Structure?
It's a way of structuring data. We are structuring this data in our RAM.

Byte = 8 bits.
A bit is a position that can store a number (0 or 1).

Int are usually stored as 4Bytes

A RAM can be thought as a continuous block of data but it has 2 components to it:
* A value: The value itself that we are saving.
* Address: The location of the value.

As we store an Array we don't always get to choose the location where is at but the thing with arrays is that they will always be continuous.

![[Pasted image 20260826134318.png]]
Strings/characters use less space(ASCII).
![[Pasted image 20260826134447.png]]
The thing is that no matter the size, arrays store elements contiguous.

### Some Arrays Properties
We use index to access elements so we don't really need to know the specific address in memory. This operation is efficient, it's **O(1)**, constant time, instantly.
`myArray[i]` for i = 0,1,2...etc.

Arrays are **Fixed-size**.  This is the biggest disadvantage of **Static Arrays**.
Languages like Python and JS don't worry about this since they use **Dynamic Arrays**.

When we say we "remove" a value, we say that we overwrite that said value.
![[Pasted image 20260826141240.png]]
Writing into any position of an Array is **O(1)**. It's constant time.
![[Pasted image 20260826141359.png]]
Similarly, removing a value is as efficient as **O(1)**. This is because we are going to that position and axing it out. We don't delete it, we overwrite it.

Inserting a value in the beginning means we need to shift all the other values. This is an operation that is more complex, so this is **O(n)**, where n is the variable, in this case it refers to the number of elements in the array (length of the array).

![[Pasted image 20260826142014.png]]

"In the worst case we might have to shift every value, that's why we use O(n). Same with removing a value in an arbitrary position."
![[Pasted image 20260826142412.png]]
For O(1) we are assuming there is an empty space to insert/remove an element.

## In-Place Algorithm

A **strict definition** is:
	*An in-place algorithm is an algorithm that does not need an extra space and produces an output in the same memory that contains the data by transforming the input 'in-place'. However, a small constant extra space used for variables is allowed.*

A more **broad definition** is:
	*In-place means that the algorithm does not use extra space for manipulating the input but may require a small though non-constant extra space for its operation. Usually, this space is O(log n), though sometimes anything in O(n) (Smaller than linear) is allowed.*
