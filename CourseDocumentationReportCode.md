## _**10. Data types, Variables, Constants and input/ output statements**_ 
Data Types in C# is Mainly Divided into 3 Categories:

1. _**Value Data Types**_

In C#, the Value Data Types will directly store the variable value in memory and it will also accept both signed and unsigned literals.
The derived class for these data types are System.ValueType. Following are different Value Data Types in C# programming language.

> 1.1 Signed & Unsigned Integral Types:

There are 8 integral types which provide support for 8-bit, 16-bit, 32-bit, and 64-bit values in signed or unsigned form
> 1.2 Floating Point Types:

There are 2 floating point data types which contain the decimal point:

* _**Float:**_ It is 32-bit single-precision floating point type. It has 7 digit Precision. 
 To initialize a float variable, use the suffix f or F. Like, float x = 3.5F;. If the suffix F or f will not use then it is treated as double.
* **Double:**_It is 64-bit double-precision floating point type. It has 14 – 15 digit Precision. 
 To initialize a double variable, use the suffix d or D. But it is not mandatory to use suffix because by default floating data types are the double type.

> 1.3 Decimal Types:

The decimal type is a 128-bit data type suitable for 
financial and monetary calculations. It has 28-29 digit Precision.
To initialize a decimal variable, use the suffix m or M. Like as, decimal x = 300.5m;. 
If the suffix m or M will not use then it is treated as double.

> 1.4 Character Types:

The character types represents a UTF-16 code unit or represents the 16-bit Unicode character.
>* Example:
 
	 // Sbyte signed integral data type
 
    using System;

    namespace ValueTypeTest {
    class GeeksforGeeks {
  
    // Main function
    static void Main()
    {
        sbyte a = 126;

        // sbyte is 8 bit
        // singned value
        Console.WriteLine(a);

        a++;
        Console.WriteLine(a);

        // It overflows here because
        // byte can hold values
        // from -128 to 127
        a++;
        Console.WriteLine(a);

        // Looping back within
        // the range
        a++;
        Console.WriteLine(a);
    }
    }
    }
>* Output
 
          126
          127
         -128
         -127 

> 1.5 Boolean Types:
It has to be assigned either true or false value.
Values of type bool are not converted implicitly or explicitly (with casts) to any other type. 
But the programmer can easily write conversion code.

>* Example:
        
        // Using Boolean data type
     using System;

    namespace ValueTypeTest {
    class GeeksforGeeks {
    
  	// Main function
    static void Main()
    {
        // boolean data type
        bool b = true;

        if (b == true)
            Console.WriteLine("Hi Geek");
    }
    }
    }
>* Output
 
      Hi Geek



2. _**Reference Data Types**_

The Reference Data Types will contain a memory address of variable value because 
 the reference types won’t store the variable value directly in memory. 
 When you create a reference type variable, such as an object or a string, you are actually storing a reference (or pointer) to 
the location in memory where the data is held. The actual data for reference types is stored on the heap. The heap is a large pool of memory used for dynamic memory allocation.
The built-in reference types are string, object.

> 2.1 String:

It represents a sequence of Unicode characters and its type name is System.String. So, string and String are equivalent.
>* Example:

    string s1 = "hello"; // creating through string keyword  
    String s2 = "welcome"; // creating through String class 
> 2.2 Object:

In C#, all types, predefined and user-defined, reference types and value types, 
inherit directly or indirectly from Object. So basically it is the base class for all the data types in C#. 
Before assigning values, it needs type conversion. When a variable of a value type is converted to object, it’s called boxing.
When a variable of type object is converted to a value type, it’s called unboxing. Its type name is System.Object.
>* Example:

    // Using Reference data types
    using System;

    namespace ValueTypeTest {

     class Geeks {
    
    // Main Function
    static void Main() 
    {
        // declaring string
        string a = "Geeks"; 
        
        // append in a
        a += "for";
        a = a + "Geeks"; 
        Console.WriteLine(a);
        
        // declare object obj
        object obj;
        obj = 20;
        Console.WriteLine(obj);
        
        // to show type of object
        // using GetType()
        Console.WriteLine(obj.GetType()); 
    }
    }
    }
>* Output
 
     GeeksforGeeks
     20
     System.Int32

3. _**Pointer Data Type**_
The Pointer Data Types will contain a memory address of the variable value. 
To get the pointer details we have a two symbols ampersand (&) and asterisk (*):

* ampersand (&): It is known as Address Operator. It is used to determine the address of a variable.
* asterisk (*): It also known as Indirection Operator. It is used to access the value of an address.

* Syntax:

       type* identifier;

* Example:

      // Valid syntax 
      int* p1, p;   

      // Invalid
      int *p1, *p;   


* Implementation:

      // Using Pointer Data Type
       using System;

      namespace Pointerprogram {
       class GFG {

       // Main function
       static void Main()
       {
        unsafe
        {
            
            // declare variable
            int n = 10;
            
            // store variable n address 
            // location in pointer variable p
            int* p = &n;
            Console.WriteLine("Value :{0}", n);
            Console.WriteLine("Address :{0}", (int)p);
              }
            }
           }
        }
>* Output:
 
     Value :10
     Address :1988374520
--------------------------------
## __*11. Arithmetic and logic operators*__

Arithmetic operators are used to perform common mathematical operations:

Operator|	Name|	Description|	Example	
--------|-------|--------------|-----------
|+ |	Addition|	Adds together two values|	x + y	
| - |	Subtraction|	Subtracts one value from another |	x - y	
|* |	Multiplication|	Multiplies two values|	x * y
|/ |	Division|	Divides one value by another|	x / y	
| %|	Modulus|	Returns the division remainder|	x % y
|++ |	Increment|   Increases the value of a variable by 1|	x++	
| --|	Decrement|	Decreases the value of a variable by 1| 	x--	

>* Example:

     // Arithmetic operators
     using System;

     class Geeks 
    {
    static void Main(string[] args)
    {
        int x = 8, y = 4;

        // Using different arithmetic operators
        Console.WriteLine("Addition: " + (x + y));
        Console.WriteLine("Subtraction: " + (x - y));
        Console.WriteLine("Multiplication: " + (x * y));
        Console.WriteLine("Division: " + (x / y));
        Console.WriteLine("Modulo: " + (x % y));
    }
    }
>* Output:
 
     Addition: 15
    Subtraction: 5
    Multiplication: 50
    Division: 2
    Modulo: 0
-----------------------------------
## _*12. Conditional statements ( if else / switch case )*_

> C# supports the usual logical conditions from mathematics:

* _Less than:_ a < b
* _Less than or equal to:_ a <= b
* _Greater than:_ a > b
* _Greater than or equal to:_ a >= b
* _Equal to:_ a == b
* _Not Equal to:_ a != b

You can use these conditions to perform different actions for different decisions.

> C# has the following conditional statements:

* Use if to specify a block of code to be executed, if a specified condition is true
* Use else to specify a block of code to be executed, if the same condition is false
* Use else if to specify a new condition to test, if the first condition is false
* Use switch to specify many alternative blocks of code to be executed

>* Example 1:

    // Use of goto in switch statement 
     using System; 

     public class Geeks 
    { 
	// Main Method 
	public static void Main(String[] args) 
	{ 
		int greeting = 2; 

		switch (greeting) { 
		case 1: 
			Console.WriteLine("Hello"); 
			goto default; 
		case 2: 
			Console.WriteLine("Bonjour"); 
			goto case 3; 
		case 3: 
			Console.WriteLine("Namaste"); 
			goto default; 
		default: 
			Console.WriteLine("Entered value is: " + greeting); 
			break; 
		} 
	} 
    } 

>*  Output:
  
    Bonjour
    Namaste
    Entered value is: 2

>* Example:
 
     using System;

     namespace MyApplication
     {
    class Program
    {
    static void Main(string[] args)
    {
      int time = 22;
      if (time < 10) 
      {
        Console.WriteLine("Good morning.");
      } 
      else if (time < 20) 
      {
        Console.WriteLine("Good day.");
      } 
      else 
      {
        Console.WriteLine("Good evening.");
      }
    }
    }
    }
>*  Output:
  
    Good evening.
---------------------------
## _*13. Looping ( for, while and do while ):*_
> Loops:

Loops can execute a block of code as long as a specified condition is reached.
Loops are handy because they save time, reduce errors, and they make code more readable.

> While Loop: 

The while loop loops through a block of code as long as a specified condition is True

>* Example:
 
    using System;

    namespace MyApplication
     {
    class Program
    {
    static void Main(string[] args)
    {
      int i = 0;
      while (i < 5) 
      {
        Console.WriteLine(i);
        i++;
      }
    }
    }
    }
>* Output:
 
       0
       1
       2
       3
       4
> The Do/While Loop:

The do/while loop is a variant of the while loop.
This loop will execute the code block once, before checking if the condition is true, 
then it will repeat the loop as long as the condition is true.

>* Example:
 
     using System;

    namespace MyApplication
    {
    class Program
    {
    static void Main(string[] args)
    {
      int i = 0;
      do 
      {
        Console.WriteLine(i);
        i++;
      }
      while (i < 5);
    }
    }
    }
>*  Output:
  
     0
     1
     2
     3
     4
> For Loop:
 
When you know exactly how many times you want to loop through a block of code, use the for loop instead of a while loop

>* Example:

    using System;

    namespace MyApplication
     {
    class Program
    {
    static void Main(string[] args)
    {
      for (int i = 0; i < 5; i++) 
      {
        Console.WriteLine(i);
      }    
    }
    }
    }
>* Output:
 
    0
    1
    2
    3
    4
------------------------------------
## __*14. Nested operations ( nested conditions and nested looping ):*__

> Nested loops:

are those loops that are present inside another loop. 
In C#, nesting of for, while, and do-while loops are allowed and you can also put any nested
loop inside any other type of loop like in a for loop you are allowed to put nested if loop.

* for Loop: The functionality of for loop is quite similar to while loop.
It is basically used when the number of times loop statements are to be executed is known beforehand.
Nesting of for loop is allowed, which means you can use for loop inside another for loop.
 
 >* Example:
  
    // C# program to illustrate nested for loop 
    using System; 

    class GFG{ 
	
    public static void Main() 
    { 
	
	// for loop within another for loop 
	// printing GeeksforGeeks 
	for(int i = 0; i < 4; i++) 
		for(int j = 1; j < i; j++) 
			Console.WriteLine("GeeksforGeeks!!"); 
     } 
     }
  >* Output:
   
    GeeksforGeeks!!
    GeeksforGeeks!!
    GeeksforGeeks!!
* while Loop:In a while loop, the test condition is given at the beginning of the loop, and all statements are executed till
the given boolean condition satisfies and when the condition becomes false, the control will be out from the while loop.
Nesting of a while loop is allowed, which means you can use while loop inside another while loop.
However, it is not recommended to use nested while loop because it is difficult to maintain and debug.

 >* Example:
  
        // C# program to illustrate nested while loop 
       using System; 

     class GFG{ 
	
     public static void Main() 
    { 
	int x = 1, y = 2; 
	
	while (x < 4) 
	{ 
		Console.WriteLine("Outer loop = {0}", x); 
		x++; 
	
		while (y < 4) 
		{ 
			Console.WriteLine("Inner loop = {0}", y); 
			y++; 
		} 
	} 
    } 
    }
>* Output:
 
    Outer loop = 1
    Inner loop = 2
    Inner loop = 3
    Outer loop = 2
    Outer loop = 3
* do-while Loop: In C#, the do-while loop is similar to the while loop with the only
difference that is, it checks the condition after executing the statements.
Nesting of a do-while loop is allowed, which means you can use a do-while loop inside another do-while loop.
>* Example:

      // C# program to illustrate nested do-while loop 
     using System; 

     class GFG{ 
	
    public static void Main() 
    { 
	int x = 1; 
	do
	{ 
		Console.WriteLine("Outer loop = {0}", x); 
		int y = x; 
	
		x++; 
				
		do
		{ 
			Console.WriteLine("Inner loop: {0}", y); 
			y++; 
		} while (y < 4); 

	} while (x < 4); 
    } 
    }
>* Output:
 
    Outer loop = 1
    Inner loop: 1
    Inner loop: 2
    Inner loop: 3
    Outer loop = 2
    Inner loop: 2
    Inner loop: 3
    Outer loop = 3
    Inner loop: 3
*  If Statement: The if statement checks the given condition.
   If the condition evaluates to be true then the block of code/statements will execute otherwise not. 
  
   >* Example:

        // Using if statement
        using System;

        public class Geeks 
       {
	   public static void Main(string[] args)
	   {
		string name = "Geek";
      
      	// Using if statement
		if (name == "Geek") {
			Console.WriteLine("GeeksForGeeks");
		}
	   }
       }
 >* Output:
  
    GeeksForGeeks
* If-else Statement:The if statement evaluates the code if the condition is true but
 what if the condition is not true, here comes the else statement.
It tells the code what to do when the if condition is false.

>* Example:
 
      // Using if-else statement
     using System;

    public class Geeks 
    {
	public static void Main(string[] args)
	{
		string name = "Geek";
      
      	// Using if-else statement
		if (name == "Geeks") {
			Console.WriteLine("GeeksForGeeksr");
		}
		else {
			Console.WriteLine("Geeks");
		}
	}
    }
   >* Output:
    
    Geeks
---------------------------------------
## _*15. Array data structure*_

An array is a group of like-typed variables that are referred to by a common name.
And each data item is called an element of the array.
The data types of the elements may be any valid data type like char, int, float, etc. and the elements are stored in a contiguous location. 
Length of the array specifies the number of elements present in the array.

The following figure shows how array stores values sequentially:
![image](https://media.geeksforgeeks.org/wp-content/uploads/20250109152710671116/Array-660.webp)
> Explanation:

The index is starting from 0, which stores value. we can also store a fixed number of values in an array.
Array index is to be increased by 1 in sequence whenever its not reach the array size.

>* Array Declaration

* Syntax:

      <Data Type>[ ] <Name_Array>
* The meaning of each one of them:

1.     <Data Type> : It define the element type of the array.
2.     [ ] : It define the size of the array.
3.     <Name_Array> : It is the Name of array. 



* Note : Only Declaration of an array doesn’t allocate memory to the array. For that array must be initialized.


>* Array Initialization:
 
As said earlier, an array is a reference type so the new keyword used to create an
instance of the array. We can assign initialize individual array elements, with the help of the index. 

* Syntax:

      type [ ] < Name_Array > = new < datatype > [size];

Here,

1. type specifies the type of data being allocated
2. size specifies the number of elements in the array
3.  Name_Array is the name of an array variable.
4. new will allocate memory to an array according to its size. 

*Example:

      // Accessing array elements using different loops
      using System;
	
     class Geeks 
     {
	// Main Method
	public static void Main()
	{
		// declares an Array of integers.
		int[] intArray;

		// allocating memory for 5 integers.
		intArray = new int[5];

		// initialize the first elements
		// of the array
		intArray[0] = 10;

		// initialize the second elements
		// of the array
		intArray[1] = 20;

		// so on...
		intArray[2] = 30;
		intArray[3] = 40;
		intArray[4] = 50;

		// accessing the elements
		// using for loop
		Console.Write("For loop :");
		for (int i = 0; i < intArray.Length; i++)
			Console.Write(" " + intArray[i]);

		Console.WriteLine("");
		Console.Write("For-each loop :");
		
		// using for-each loop
		foreach(int i in intArray)
			Console.Write(" " + i);

		Console.WriteLine("");
		Console.Write("while loop :");
		
		// using while loop
		int j = 0;
		while (j < intArray.Length) {
			Console.Write(" " + intArray[j]);
			j++;
		}

		Console.WriteLine("");
		Console.Write("Do-while loop :");
		
		// using do-while loop
		int k = 0;
		do
		{
			Console.Write(" " + intArray[k]);
			k++;
		} while (k < intArray.Length);
	}
     }
* Output:

      For loop : 10 20 30 40 50
      For-each loop : 10 20 30 40 50
      while loop : 10 20 30 40 50
      Do-while loop : 10 20 30 40 50
----------------------------------------------
## _*16. Functions in CSharp ( built-in ):*_
> Built-in Functions:

These functions are available by .Net Framework to perform common tasks, ranging from 
mathematical operations to string manipulation, array handling, and more.
> 1. Math Functions: 
  
The Math class provides various mathematical functions.

• Math.Abs: Returns the absolute value of a number.

        int value = -10; 
        int absoluteValue = Math.Abs(value); // absoluteValue = 10 
• Math.Pow: Raises a number to a specified power. 

        double result = Math.Pow(2, 3); // result = 8 
• Math.Sqrt: Returns the square root of a number. 

       double squareRoot = Math.Sqrt(16); // squareRoot = 4 
* Math.Round:  a floating-point number to the nearest integer or specified number of decimal places. 

               double rounded = Math.Round(4.56789, 2); // rounded = 4.57
> 2. String Functions:
  
  The String class provides methods to manipulate strings. 

  • string.Length: Gets the length of a string. 

      string message = "Hello, world!"; 
    int length = message.Length; // length = 13 
* string.ToUpper and string.ToLower: Convert a string to uppercase or lowercase.

        string upper = message.ToUpper(); // upper = "HELLO, WORLD!" 
        string lower = message.ToLower(); // lower = "hello, world!"
* string.Contains: Determines whether a string contains a specified substring. 

           bool contains = message.Contains("world"); // contains = true 
• string.Split: Splits a string into an array of substrings based on a delimiter.

           string[] words = message.Split(' '); // words = ["Hello,", "world!"] 

> 3. Date and Time Functions:
  
The DateTime class provides functions to work with dates and times.
   * DateTime.Now: Gets the current date and time. 
   
                  DateTime now = DateTime.Now; 
• DateTime.Today: Gets the current date with the time component set to 00:00:00.

                  DateTime today = DateTime.Today
* DateTime.ToString: Converts the date and time to a string in a specified format. 

       string formattedDate = now.ToString("yyyy-MM-dd HH:mm:ss"); // formattedDate = "2024-08-18 
       15:30:00" 
>  4. Array Functions:
   
   C# arrays have several built-in methods. 

• Array.Sort: Sorts the elements of an array. 

              int[] numbers = { 3, 1, 4, 1, 5 }; 
               Array.Sort(numbers); // numbers = { 1, 1, 3, 4, 5 } 
• Array.Reverse: Reverses the sequence of the elements in an array. 

              Array.Reverse(numbers); // numbers = { 5, 4, 3, 1, 1 } 
• Array.IndexOf: Searches for the specified object and returns the index of its first occurrence 
in an array. 

           int index = Array.IndexOf(numbers, 4); // index = 1
> 5. Console Functions:
  
The Console class is used for basic input/output operations. 

• Console.WriteLine: Writes the specified data, followed by the current line terminator, to the 
console. 

           Console.WriteLine("Hello, world!"); 
• Console.Write: Writes the specified data to the console without appending a new line.

            Console.Write("Enter your name: "); 
• Console.ReadLine: Reads the next line of characters from the standard input stream. 

            string name = Console.ReadLine();
> 6. Type Conversion Functions:
  
C# provides several built-in methods for converting between types. 

• Convert.ToInt32: Converts a specified value to a 32-bit signed integer. 

           string numberString = "123"; 
           int number = Convert.ToInt32(numberString); // number = 123 
• Convert.ToDouble: Converts a specified value to a double-precision floating-point number. 

              string doubleString = "123.45"; 
              double doubleNumber = Convert.ToDouble(doubleString); // doubleNumber = 123.45 
 
• Convert.ToString: Converts a specified value to a string. 

               int num = 123; 
         string numString = Convert.ToString(num); // numString = "123" 
• int.Parse and int.TryParse: Convert a string representation of a number to its integer 
equivalent. 

             int parsedNumber = int.Parse("456"); // parsedNumber = 456 
             bool success = int.TryParse("456"); // success = true
> 8. Random Number Functions:
  
The Random class is used to generate random numbers.

• Random.Next: Returns a random integer. 

          Random random = new Random(); 
            int randomNumber = random.Next(); // randomNumber = any integer 
            int randomInRange = random.Next(1, 10); // randomInRange = integer between 1 and 9 
• Random.NextDouble: Returns a random floating-point number between 0.0 and 1.0 

           double randomDouble = random.NextDouble(); // randomDouble = value between 0.0 and 1.0
-----------------------------------------------
## _*17. Errors in programming:*_
In programming, errors can generally be categorized into three main types: syntax errors, runtime 
errors, and logical errors. Understanding these error types is crucial for effective debugging and 
writing robust code. Let's explore each type with examples and how to handle them in C#. 
 
> 1. Syntax Errors:
  
Syntax errors occur when the code violates the grammatical rules of the programming language. 
These errors are usually detected by the compiler before the program runs.

> 2. Runtime Errors:
  
Runtime errors occur while the program is running, usually because of operations that are not 
logically valid at runtime, such as dividing by zero, accessing an array out of bounds, or attempting 
to use a null reference.
> 3.  Logical Errors:
   
Logical errors occur when the program compiles and runs, but the output is not what you expected. 
These errors are the most difficult to detect because the program doesn't crash or show any 
immediate signs of error.

>* Example 1:
 
    using System;

      namespace MyApplication
    {
    class Program
    {
    static void Main(string[] args)
    {
      try
      {
        int[] myNumbers = {1, 2, 3};
        Console.WriteLine(myNumbers[10]);
      }
      catch (Exception e)
      {
        Console.WriteLine(e.Message);
      }    
    }
    }
    }
>* Output:
 
     Index was outside the bounds of the array.
>* Example 2:
 
     using System;

      namespace MyApplication
     {
    class Program
    {
    static void Main(string[] args)
    {
      try
      {
        int[] myNumbers = {1, 2, 3};
        Console.WriteLine(myNumbers[10]);
      }
      catch (Exception e)
      {
        Console.WriteLine("Something went wrong.");
      }    
    }
    }
    }
>* Output:
 
     Something went wrong.
>* Example 3:
 
    using System;

    namespace MyApplication
    {
     class Program
    {
    static void Main(string[] args)
    {
      try
      {
        int[] myNumbers = {1, 2, 3};
        Console.WriteLine(myNumbers[10]);
      }
      catch (Exception e)
      {
        Console.WriteLine("Something went wrong.");
      }  
      finally
      {
        Console.WriteLine("The 'try catch' is finished.");
      }  
    }
    }
    }
>* Output:
       
        Something went wrong.
      The 'try catch' is finished.


