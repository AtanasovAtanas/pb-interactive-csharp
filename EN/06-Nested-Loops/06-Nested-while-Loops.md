[slide]
# Nested While Loops
The use of nested `while` loops is very similar to the one of the `for`.

Here is the syntax in C#:
```csharp
while (condition) 
{
  // Outer Loop 
  while (condition) 
  {
    // Inner Loop
    
    // Statements
  }
}
```

# Example

```csharp
int i = 0;
while (i < 2)
{
  Console.WriteLine($"Value of i: {i}");
  int j = 1;
  i++;

  while (j < 2)
  {
    Console.WriteLine($"Value of j: {j}");
    j++;
  }
}

// Output
// Value of i: 0 
// Value of j: 1 
// Value of i: 1 
// Value of j: 1 
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
      int i = 1;

      while (i <= height)
      {
          int j = 1;
          while (j <= i)
          {
              Console.Write("*");
              j++;
          }

          Console.WriteLine();
          i++;
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

[vimeo-video videoId="342526930" startTimeInSeconds="4421" endTimeInSeconds="5562" /]

[/slide]