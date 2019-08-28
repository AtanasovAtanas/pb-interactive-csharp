[slide]
# Console (Terminal)
Generally, the **system console** represents a text terminal, which means that it accepts and visualizes just **text** without any graphical elements like buttons, menus, etc. 

It usually looks like a black colored window like this one:

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.Console-example.png"/]

In most operating systems, the **console** is available as a standalone application on which we write console commands. 

It is called a **Command Prompt** in Windows, and a **Terminal** in Linux and Mac. 

The console runs console applications. They read text from the command line and print text on the console. In this book we are going to learn programming mostly through creating **console applications**.

In the next examples we will **read data** (like integers, floating-point numbers and strings) from the console and will **print data** on the console (text and numbers).
[/slide]

[slide]
# Reading User Input
Everything we read from the console comes as a **string**. 

In order to read an integer (not a float) number from the console, we have to declare a variable, declare the number type and use the standard command for reading a text line from the system console `Console.ReadLine()` and after that convert the text line into an integer number using `int.Parse(text)`.

Here are ways to read user input from the console:
```csharp
string name = Console.ReadLine();
```
[/slide]

[slide]
# Formatting Output
Formatting text with **placeholders**

```csharp
string firstName = "John";
string lastName = "Doe";
Console.WriteLine("{0} {1}", firstName, lastName);
// John Doe
```

Formatting numbers with **placeholders**
```csharp
double a = 5.123;
double b = 6.456;
Console.WriteLine("{0:F2}", a + b); // 11.58
```

Formatting output using **string interpolation**
  * **String interpolation** provides a **more readable** and **convenient** syntax to create **formatted strings**
  * To identify a string as an interpolated string, prepend it with the **`$`** symbol
  * **Parameters** are put directly in **placeholders**
```csharp
int day = 12;
string month = "April";
int year = 2018
Console.WriteLine($"{day}-{month}-{year}");
// 12-April-2018
```
[/slide]

[slide]
# Reading Integers
In order to read an **integer** (not a float) **number** from the console, we have to **declare a variable**, declare the **number type** and use the standard command for **reading a text line** from the system console `Console.ReadLine()` and after that **convert the text line into an integer number** using `int.Parse(text)`:

```cs
int num = int.Parse(Console.ReadLine());
```

The above line of C# code **reads an integer** from the first line on the console.

Try to write a wrong number, for example **"hello"**. 

You will get an error message during runtime (exception). This is normal. 

Later on, we will find out how we can catch these kinds of errors and make the user enter a number again.

# Examole: Calculating a Square Area
This code demonstrates how we can calculate the square area by the given length of the side:
```cs
Console.Write("a = ");              
int a = int.Parse(Console.ReadLine());
int area = a * a;
Console.Write("Square area = ");
Console.WriteLine(area);
```

Here is how the program would work when we have a square with a side length equal to 3:

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.Square-area-01.jpg"/]
[/slide]

[slide]

# Reading Floating-Point Numbers
To read a **floating-point number** (fractional number, non-integer) from the console use the following command:
```cs
double num = double.Parse(Console.ReadLine());
```

The above C# code first reads a **text line** from the console, then converts (parses) it to a **floating-point number**.

# Example: Converting Inches into Centimeters
Let's write a program that reads a floating-point number in inches and converts it to centimeters:
```cs
Console.Write("Inches = ");              
double inches = double.Parse(Console.ReadLine());
double centimeters = inches * 2.54;
Console.Write("Centimeters = ");
Console.WriteLine(centimeters);
```

Let's start the program and make sure that when a value in inches is entered, we obtain a correct output in centimeters:

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.Inches-to-centimeters-01.jpg"/]

Note that if you enter and **invalid number**, e.g. **"asfd"**, the program will crash with an error message (exception). We will learn how to handle exceptions in later courses.
[/slide]

[slide]
# Problem: Greeting
[code-task title="Greeting" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
    // Write code here
  }
}
```
[/code-editor]
[task-description]
Write a **program**, which:

  * Reads a user input: **name**, from the console
  * Prints "Hello, \{name\}", where {**name**} is the **user input**
[/task-description]
[tests]
[test]
[input]
John
[/input]
[output]
Hello, John
[/output]
[/test]
[test]
[input]
Marie
[/input]
[output]
Hello, Marie
[/output]
[/test]
[test]
[input]
asd
[/input]
[output]
Hello, asd
[/output]
[/test]
[test]
[input]
George
[/input]
[output]
Hello, George
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Greeting
[code-task title="Greeting" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
    string name = Console.ReadLine();
    Console.Write("Hello, ");
    Console.WriteLine(name);
  }
}
```
[/code-editor]
[task-description]
Write a **program**, which:

  * Reads a user input: **name**, from the console
  * Prints "Hello, \{name\}", where {**name**} is the **user input**
[/task-description]
[tests]
[test]
[input]
John
[/input]
[output]
Hello, John
[/output]
[/test]
[test]
[input]
Marie
[/input]
[output]
Hello, Marie
[/output]
[/test]
[test]
[input]
asd
[/input]
[output]
Hello, asd
[/output]
[/test]
[test]
[input]
George
[/input]
[output]
Hello, George
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Concatenating Text and Numbers
Besides for summing up numbers, the operator `+` is also used for **joining pieces of text** (concatenation of two strings one after another). 

In programming, joining two pieces of text is called **"concatenation"**. 

Here is how we can concatenate a text with a number by the `+` operator:

```cs
string firstName = "John";
string lastName = "Doe";
int age = 19;
var str = firstName + " " + lastName + " @ " + age;
Console.WriteLine(str);  // John Doe @ 19
```

# Examples: Concatenating Text and Numbers
Here is another **example** of concatenating text and numbers:
```cs
double a = 1.5;
double b = 2.5;
string sum = "The sum is: " + a + b;
Console.WriteLine(sum);  // The sum is: 1.52.5
```

Did you notice **something strange**? 

Maybe you expected the numbers `a` and `b` to be summed? 

Actually, the concatenation works from right to left and the result above is absolutely correct. 

If we want to sum the numbers, we have to use **brackets**, in order to change the order of execution of the operations:
```cs
double a = 1.5;
double b = 2.5;
string sum = "The sum is: " + (a + b);
Console.WriteLine(sum);  // The sum is: 4
```
[/slide]

[slide]
# Video

[vimeo-video videoId="341512905" startTimeInSeconds="3817" endTimeInSeconds="5967" /]

[/slide]