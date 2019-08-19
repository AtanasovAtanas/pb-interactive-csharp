[slide]
# Nested While Loops

A nested while loop is a **while statement inside** another **while statement**. 

In a nested while loop, one iteration of the outer loop is first executed, after which the inner loop is executed. 

The execution of the inner loop continues till the condition described in the inner loop is satisfied. 

Once the condition of the inner loop is satisfied, the program moves to the next iteration of the outer loop.

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

**Example**

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
[code-task title="Triangle of Stars with While" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[code-io /]
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
[code-task title="Triangle of Stars with While" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[code-io /]
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