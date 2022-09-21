## Arrays Vs ArrayLists
**Important Vocabulary:**
- Element: An item in an array
- Index: The location of an item in an array. Indexes start at 0.
  -  For example, the indexes of this array {214, 5432, 124} are {0, 1, 2}
  
**The Jist:**
- Arrays have a set length, often with pre defined elements
  - Good for if your memory has limits/constraints, or you have a pre defined list you need to loop through
- Arraylists have no defined length, and can be infinitely long
  - Good for shopping lists, customer invoices, file I/O

## Array Syntax
*Note: 2D Arrays are not covered in this document, this is more general. Please see INSERTDOC for info on 2D arrays*  

**Syntax:**  
`DataType[] NAME = new DataType[NUM OF ITEMS];` OR `DataType[] NAME = {elements of that datatype, separated by commas};`

**Methods/Common Uses:**  
Example array for reference: `int[] arrTest = {2143, 43, 543, 12, 564}`
- `NAME[index]` : Accesses an element in an array at a specific index
  - Ex: `arrTest[0]` is 2143 
