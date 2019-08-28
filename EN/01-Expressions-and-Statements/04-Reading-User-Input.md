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

# Reading User Input
A program which **reads** a name from the console and **prints** it:

```csharp
string name = Console.ReadLine();
Console.WriteLine(name);
```
The result from the execution would be:

[image src="https://github.com/AlenPaunov/pb-interactive-course/blob/01-expressions-and-statements/assets/expressions-and-statements-2.png"/]

[/slide]

[slide]

# Reading Integers
Reading an integer number:

```csharp
int num = int.Parse(Console.ReadLine());
```
Example: 

  * Calculating square's area by given side **a**
  ```csharp
  int a = int.Parse(Console.ReadLine());
  int area = a * a;
  Console.WriteLine(area);
  ```

[/slide]

[slide]

# Reading Floating-Point Numbers
Reading a floating-point number:

```csharp
double num = double.Parse(Console.ReadLine());
```
Example: 

  * Convert inches to centimeters
```csharp
double inches = double.Parse(Console.ReadLine());
double centimeters = inches * 2.54;
Console.WriteLine(centimeters);
```
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
We can use the **+** to append strings:

```csharp
string firstName = "John";
string lastName = "Doe";
int age = 34;
string str = firstName + " " + lastName + " | " + age;
Console.WriteLine(str); // John Doe | 34
```

When using the **+** sign with numbers, an addition operation is performed:
```csharp
int a = 5;
int b = 11;
string str = "a + b = " + a + b;
Console.WriteLine(str); // a + b = 511
```
[/slide]

[slide]
# Video

[vimeo-video videoId="341512905" startTimeInSeconds="3817" endTimeInSeconds="5967" /]

[/slide]