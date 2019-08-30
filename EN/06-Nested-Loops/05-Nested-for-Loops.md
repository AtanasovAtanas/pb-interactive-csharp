[slide]
# Nested for Loops
Statements that consist of several ** for loops** located **inside each other**

**Nested for loops** are used:

* To execute an **action**, which **executes** multiple **actions**
* To make more **complex** calculations and variations

These are `for` loops nested in one another:
```csharp
for (int i = 1; i <= n; i+=3) 
{
   for (int j = 1; j <= n; j+=3)
   {
      for (int k = 1; k <= n; k+=3)
      {
        // ...
      }
   }
}
```

The syntax for a **nested for loop in C#** is as follows:
```csharp
for (variable initialization; condition; increment) 
{
  // Outer Loop 
  for (variable initialization; condition; increment) 
  { 
    // Inner Loop

    // Statements
  }
}
```
Here is an example C# program:
```csharp
int a = 3;
int b = 3;
for (int i = 0; i < a; i++) 
{
  Console.WriteLine("i = " + i);
  for (int j = 0; j < b; j++)
  {
    // Print "j = " and value of j
  }
}
```
[/slide]

[slide]
# Problem: Triangle of Stars
[code-task title="Triangle of Stars" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which:

* Reads the **height** of a triangle from the console
* Prints a **triangle of stars**
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
*
**
***
****
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|*|
||**|
||***|
||****|
||*****|
[/slide]

[slide]
# Solution: Triangle of Stars
[code-task title="Triangle of Stars" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int height = int.Parse(Console.ReadLine());
      for (int i = 1; i <= height;  i++)
      {
          for (int j = 1; j <= i; j++)
          {
              Console.Write("*");
          }
          Console.WriteLine();
      }
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the **height** of a triangle from the console
* Prints a **triangle of stars**
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
*
**
***
****
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|*|
||**|
||***|
||****|
||*****|
[/slide]

[slide]
# Video

[vimeo-video videoId="342526930" startTimeInSeconds="3765" endTimeInSeconds="4420" /]

[/slide]