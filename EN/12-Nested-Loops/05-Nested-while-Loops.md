[slide]
# Nested while Loops
The use of nested `while` loops is very similar to the one of the `for`. Here is the syntax in C#:
```csharp
// Outer Loop 
while (condition) 
{
    // Inner Loop
  while (condition) 
  {
    // Statements
  }
}
```

# Example

```cs live
int row = 0;
int n = 5;
while (row < n)
{
  Console.WriteLine($"Row: {row}");
  int col = 1;
  row++;

  while (col < n)
  {
    Console.WriteLine($"  Col: {col}");
    col++;
  }
}
```
[/slide]

[slide]
# Problem: Triangle of Stars with While
[code-task title="Triangle of Stars with While" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
# Solution: Triangle of Stars with While
[code-task title="Triangle of Stars with While" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
      int height = int.Parse(Console.ReadLine());
      int row = 1;

      while (row <= height)
      {
          int col = 1;
          while (col <= row)
          {
              Console.Write("*");
              col++;
          }

          Console.WriteLine();
          row++;
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

[vimeo-video videoId="342526930" startTimeInSeconds="4421" endTimeInSeconds="5562" /]

[/slide]