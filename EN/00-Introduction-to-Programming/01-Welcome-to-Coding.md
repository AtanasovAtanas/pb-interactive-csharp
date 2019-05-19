[slide]
# What is Coding?
**Coding** means to give **commands** to tell the computer what to do

Sample command:
```csharp
Console.WriteLine("I am coding");
```
A **computer program** is a sequence of commands
```csharp
Console.WriteLine("First command");
Console.WriteLine("Second command");
Console.WriteLine("Third command");
```
[/slide]

[slide]
# Commands in C# – Examples 
Calculate an expression and print its value:
```csharp
Console.WriteLine(5 + 5);
```
Plays the "A" sound (works in Windows only)
```csharp
Console.Beep(432, 500);
```
Print the numbers from 1 to 100
```csharp
for (int i = 1; i <= 100; i ++)
   Console.WriteLine(i);
```
[/slide]

[slide]
# Programming and Algorithms 
**Programming** means writing computer programs (commands)

* Using certain **programming language**, such as C# or Python

**Algorithm** == a sequence of commands that achieves certain result

Programming is done by **programmers** (developers)

Programmers use IDE (like Visual Studio) to:

* **Write** the code
* **Run** and test the code
* Find a fix **bugs** (debug the code)
[/slide]

[slide]
# Computer Program – Example
Sample C# program (sequence of C# commands):

```csharp
var size = 5;
Console.WriteLine("Size = " + size);
Console.WriteLine("Area = " + size * size);
```

[image src="https://github.com/tany1610/programming-basics-interactive-csharp/blob/master/assets/intro-to-programming-1.png"/]
[/slide]

[slide]
# Complete Computer Program
Sample complete C# program (class + method + commands):
```csharp
using System;

class SquareArea
{
  public static void Main()
  {
    var size = 5;
    Console.WriteLine("Size = " + size);
    Console.WriteLine("Area = " + size * size);
  }
}
```
[/slide]

[slide]
# Console-Based C# Program – Example
C# program, which converts from USD to EUR

```csharp
using System;

class SquareArea
{
  public static void Main()
  {
    var dollars = int.Parse(Console.ReadLine());
    var euro = dollars * 0.883795087;
    Console.WriteLine("Euro: " + euro);
  }
}
```
[/slide]