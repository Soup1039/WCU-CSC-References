# Basic Java References & Guide
Use this guide if you have general questions, or need a refresher on some of the basics.

## Starting a program
```
public class FILENAME {
    public static void main (String[] args) {
    
    }
} 
```
Note: No matter what you do in the file, you *always* need a public class encapsulating your program! Otherwise the computer has no idea how to find the file.

## Import Statements
``` 
import java.WHATEVER;
public class FILENAME {
    };
```

## Variable Types And Usages
`int` : integer  
`double` : either an integer or a non-whole number. Any whole numbers represented this way will be listed as "number.0"  
`String` : any "string" of characters  
`char` : one character  
`ArrayList<DATATYPE> NAME = new ArrayList<DATATYPE>()` : ArrayList that can be used to create a dynamic array (see file about arrays vs arraylists for detailed descriptions)  
`DATATYPE[] name = {elements separated by commas, of the specified data type}` : Array with defined elements  
`DATATYPE[] name = new DATATYPE[number of elements]` : Creates an array with a number of elements that do not have values  

## Using Print Statements
System.out.println("TEXT"); : Text statement that takes up a full line, and will make the next print statements go onto a new line  
System.out.print("TEXT"); : A print statement that takes up a portion of a line  

## PrintF Statements
Syntax:
`System.out.printf("Words words ACCESSOR words", variables with type of accessor)`  

Accessors:
- `%s` --> Strings
- `%d` --> integers  
- `%f` --> floats

To give the accessor a specific width, do %NumOfCharactersDataType . If you put a negative before it, it'll left align. Otherwise it will right align by default. Ex:  
Left-aligned code:  
`String test = "Hi World!";`  
`System.out.printf("This is a left aligned string: %-10s", test);`

For floats, you can round the digits off by doing `.2` for two places. So, ex: `%-8.2f` for a float that is left-aligned, takes up 8 characters, and rounds to 2 places 

## Loops
**While:**  
- Runs infinitely until condition is false  
- Good for updating canvases, checking if an users input is out of range  

Syntax:
```
while (condition) {
     code here
} 
```

**Do While:**
- Always runs at least once, even if condition is false  
- Good for printing menus  

Syntax:  
```
do {

} while (condition);
```

**For Loop:**  
-Runs a set number of times, aka iterations
-Good for looping through array values, lists, things like that

Syntax:
*Note: I have used i here, but that can be replaced with any name, since it is a var.*
```
for (int i = 0; condition; what to do each iteration; {

} 
```

Example:
``` 
for (int i = 0; i< 10; i++) {  
      this loop will iterate ten times, each time increasing by 1. i starts at 0, then increases to 1 after it loops,  
      so on and so forth until it reachs 10. Since 10 < 10 is false, the loop stops.  
} 
```
