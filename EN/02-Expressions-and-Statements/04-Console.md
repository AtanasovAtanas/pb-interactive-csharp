# Console (Terminal)

[slide]
# Video

[vimeo-video videoId="341512905" startTimeInSeconds="3817" endTimeInSeconds="5967" /]

[/slide]

[slide]
# Console (Terminal)
Generally, the **system console** represents a text terminal, which means that it accepts and visualizes just **text** without any graphical elements like buttons, menus, etc. 

It usually looks like a black colored window like this one:

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/00.Console-example.png"/]

In most operating systems, the **console** is available as a standalone application on which we write console commands. 

It is called a **Command Prompt** in Windows, and a **Terminal** in Linux and Mac. 

The console runs console applications. They read text from the command line and print text on the console. We are going to learn programming mostly through creating **console applications**.

In the next examples we will **read data** (like integers, floating-point numbers and strings) from the console and will **print data** on the console (text and numbers).
[/slide]

[slide]
# Printing and Formatting Text and Numbers

## Using `Console.Write(…)` and `Console.WriteLine(…)`
Work with these methods is easy because they can print all the basic types (string, numeric and primitive types).

Here are some examples of printing various types of data:
```cs live
Console.WriteLine("Hello World");
Console.WriteLine(5);
Console.WriteLine(3.14159265358979);
```

As we see by using `Console.WriteLine(…)` it is possible to print various data types because for each type there is a predefined version of the method `WriteLine(…)` in the `Console` class.

The difference between `Write(…)` and `WriteLine(…)` is that the `Write(…)` method prints on the console what it is provided between the parentheses but does nothing in addition while the method `WriteLine(…)` means directly **"write line"**. 

This method does what the `Write(…)` one does but in addition goes to a new line. 

In fact the method does not print a new line but simply puts a **"command" for moving** cursor to the position where the new line starts (this command consists of the character `\r` followed by `\n`).

Here is an example, which illustrates the difference between `Write(…)` and `WriteLine(…)`:
```cs live
Console.WriteLine("I love");
Console.Write("this ");
Console.Write("course!");
```

We notice that the output of this example is printed on two lines, even though the code is on three. 

This happens because on the first line of code we use `WriteLine(…)` which prints **"I love"** and then goes to a new line. 

In the next two lines of the code uses the `Write(…)` method, which prints without going on a new line and thus the words **"this"** and **"course!"** remain on the same line.

## Formatting
In C#, when printing a text, numbers and other data on the console, **we can join them** by using templates `{0}`, `{1}`, `{2}` etc. 

In programming, these templates are called **placeholders**. This is a simple example:
```cs live
Console.WriteLine("{0} + {1} = {2}", 3, 5, 3 + 5);
```

The placeholders `{0}`, `{1}` and `{2}` are replaced by the expressions, given after the text.

## Using the Dollar String Interpolation
We can format text in C# using also the following $ syntax. It provides simplifies text formatting:
```cs live
double a = 4.5;
Console.WriteLine($"Square size = {a}");
Console.WriteLine($"Square area = {a * a}");
```

The `$` prefix before a string in C# enables the so called **"string interpolation"**: replacing all expressions, staying in curly brackets `{ }` in the text with their values.
[/slide]

[slide]
# Reading User Input
To read a **text** (string) from the console, again, we have to **declare a new variable** and use the standard **command for reading a text from the console**:
```cs 
string str = Console.ReadLine();
```

By default, the `Console.ReadLine(…)` method returns a **text result** – a text line, read from the console.
- After you read a text from the console, additionally, you can **parse the text** to an integer by `int.Parse(…)` or a floating-point number by `double.Parse(…)`.
- If parsing to a number is not done, **each number** will simply be **text**, and we **cannot do** arithmetic operations with it.

# Example: Home Town
Let's write a program that asks the user for their home town and prints the text `"I am from {homeTown}!"`.

```cs
string homeTown = Console.ReadLine();
Console.WriteLine($"I am from {homeTown}!");
```

In this case the `{homeTown}` expression is replaced with the value of the variable `homeTown`. 

If we enter **"Sofia"**, the output will be as follows:
```
I am from Sofia!
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

# Example: Calculating a Square Area
This code demonstrates how we can calculate the square area by the given length of the side:
```cs
Console.Write("a = ");              
int a = int.Parse(Console.ReadLine());
int area = a * a;
Console.Write("Square area = ");
Console.WriteLine(area);
```

Here is how the program would work if we had a square with a side length equal to 3:

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

Note that if you enter and **invalid number**, e.g. **"asfd"**, the program will crash with an error message (exception). 

We will learn how to handle exceptions in later courses.
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
# Description
Write a **program**, which:

  * Reads a user input: **name**, from the console
  * Prints "Hello, \{name\}", where {**name**} is the **user input**
# Example
## Input
- Peter
## Output
- Hello, Peter
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
[code-io/]
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
# Description
Write a **program**, which:

  * Reads a user input: **name**, from the console
  * Prints "Hello, \{name\}", where {**name**} is the **user input**
# Example
## Input
- Peter
## Output
- Hello, Peter
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
[code-io/]
[/code-task]
[/slide]

[slide]
# Concatenating Text and Numbers
Besides for summing up numbers, the operator `+` is also used for **joining pieces of text** (concatenation of two strings one after another). 

In programming, joining two pieces of text is called **"concatenation"**. 

Here is how we can concatenate a text with a number by the `+` operator:

```cs live
string firstName = "John";
string lastName = "Doe";
int age = 19;
var str = firstName + " " + lastName + " @ " + age;
Console.WriteLine(str);  // John Doe @ 19
```

# Examples: Concatenating Text and Numbers
Here is another **example** of concatenating text and numbers:
```cs live
double a = 1.5;
double b = 2.5;
string sum = "The sum is: " + a + b;
Console.WriteLine(sum);  // The sum is: 1.52.5
```

Did you notice **something strange**? Maybe you expected the numbers `a` and `b` to be summed? 

Actually, the concatenation works from right to left and the result above is absolutely correct. 

If we want to sum the numbers, we have to use **brackets**, in order to change the order of execution of the operations:
```cs live
double a = 1.5;
double b = 2.5;
string sum = "The sum is: " + (a + b);
Console.WriteLine(sum);  // The sum is: 4
```
[/slide]