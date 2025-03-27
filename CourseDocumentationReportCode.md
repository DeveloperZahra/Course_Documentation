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





    

