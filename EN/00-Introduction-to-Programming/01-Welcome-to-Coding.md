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

## Programming
**Programming** means writing computer programs (commands). 

Computer programs usually execute some algorithm. 

Algorithms are a sequence of steps, necessary for the completion of a certain task and for gaining some expected result, something like a "recipe". 

We need to use a certain **programming language**, such as C# or Python, to write it.

## Algorithms
**Algorithm** is a sequence of commands that achieves certain result

In programming the computer programs execute algorithms, necessary for the completion of a certain task. 

For example, to arrange a sequence of numbers in an ascending order, an algorithm is needed, e.g. find the smallest number and print it, then find the smallest number among the rest of the numbers and print it, and this is repeated until there are no more numbers left.
[/slide]

[slide]
# Computer Programs
Computer programs represent a sequence of commands that are written in certain programming language, 
like C#, Java, JavaScript, Python, C++, PHP, C, Ruby, Swift, Go or another.

Sample C# program (sequence of C# commands):

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

The above program defines a class SquareArea, holding a method Main(), which holds a sequence of 3 commands:
 * Declaring and assigning a variable: var size = 5;
 * Calculating and printing an expression: Console.WriteLine("Size = " + size);
 * Calculating and printing an expression: Console.WriteLine("Area = " + size * size);

The result (output) from the above program is as follows:
```csharp
Size = 5
Area = 25
```

We shall explain in detail how to write programs in C# and why we need to define a class and why we need to define a method Main() a bit later.

In order to write commands, we should know the syntax and the semantics of the language which we are working with, in our case – C#. 

Therefore, we are going to get familiar with the syntax and the semantics of the language C#, and with programming generally by learning step by step  code writing from the simpler to the more complex programming constructions.

[image src="https://github.com/AlenPaunov/pb-interactive-csharp/blob/master/assets/intro-to-programming-1.png"/]
[/slide]

[slide]
# Console-Based C# Program – Example
Let's look at a simple program that reads from the user some amount of money in U.S. Dollars (USD) - an integer, converts it into Euro (EUR) by dividing it by the Euro's rate and prints the obtained result. 

This is a program of 3 consecutive commands:

```csharp
using System;

class DollarsToEuroConverter 
{
    static void Main()
    {
        var dollars = int.Parse(Console.ReadLine());
        var euro = dollars * 0.883795087;
        Console.WriteLine(euro);
    }
}
```
[/slide]

[slide]
# Video

[vimeo-video videoId="342590118" startTimeInSeconds="1770" endTimeInSeconds="2920" /]

[/slide]

[html]
<style>
  . this-is-custom-element {
      background-color: yellow;
   }
   .pull-left {
       float: left;
   }
</style>
<div class="this-is-custom-element">
  <div class="pull-left">This is left</div>
</div>
<script>
  document.querySelector('.this-is-custom-element')
       .addEventListener('click', () => { alert('It works') });
</script>
[/html]