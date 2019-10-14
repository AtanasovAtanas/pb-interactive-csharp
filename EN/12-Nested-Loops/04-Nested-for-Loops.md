[slide]
# Nested for Loops
Statements that consist of several **for loops** located **inside each other**

**Nested for loops** are used:

* To execute an **action**, which **executes** multiple **actions**
* To make more **complex** calculations and variations

The syntax for a **nested for loop in C#** is as follows:
```csharp
  // Outer Loop 
for (variable initialization; condition; increment) 
{
    // Inner Loop
  for (variable initialization; condition; increment) 
  { 

    // Statements
  }
}
```
T
hese are 3 `for` loops nested in one another:
```cs live
int n = 5;
for (int i = 1; i <= n; i += 3) 
{
    for (int j = 1; j <= n; j += 3)
    {
        for (int k = 1; k <= n; k += 3)
        {
            Console.WriteLine($"{i}{j}{k}");
        }
    }
}
```
# Example
Here is an example C# program:
```cs live
int a = 3;
int b = 3;

for (int row = 0; row < a; row++) 
{
    Console.WriteLine("row = " + row);

    for (int col = 0; col < b; col++)
    {
        Console.WriteLine($"  col = " + col);
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
# Description
Write a program, which:

* Reads the **height** of a triangle from the console
* Prints a **triangle of stars**
# Example
## Input
- 5
## Output
```
*
**
***
****
*****
```
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
[code-io/]
[/code-task]

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
      for (int row = 1; row <= height; row++)
      {
          for (int col = 1; col <= i; col++)
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
# Description
Write a program, which:

* Reads the **height** of a triangle from the console
* Prints a **triangle of stars**
# Example
## Input
- 5
## Output
```
*
**
***
****
*****
```
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
[code-io/]
[/code-task]

[/slide]

[slide]
# Video

[vimeo-video videoId="342526930" startTimeInSeconds="3765" endTimeInSeconds="4420" /]

[/slide]