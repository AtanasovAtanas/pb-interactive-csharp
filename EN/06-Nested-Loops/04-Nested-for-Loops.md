[slide]
# Nested for Loops
Statements that consist of several **loops** located **inside each other**

**Nested loops** are used:

* To execute an **action**, which **executes** multiple **actions**
* To make more **complex** calculations and variations

---

A nested loop is a construction where in the body of one loop (**outer one**) stays another loop (**inner one**). 

In each iteration of the outer loop, the whole inner loop is executed. 

This happens in the following way:

* When nested loops start executing, the outer loop starts first: 
  * the controlling variable is initialized and after a check for ending the loop the code in its body is executed.
* After that, the inner loop is executed. 
  * The controlling variables start position is initialized, a check for ending the loop is made and the code in its body is executed.
* When reaching the specified value for ending the loop, the program goes back one step up and continues executing the previous (outer) loop.
* The controlling variable of the outer loop changes with one step, a check is made to see if the condition for ending the loop is met and a new execution of the nested (inner) loop is started.

This is repeated until the variable of the outer loop meets the condition to end the loop.

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
[/slide]

[slide]
# Nested for Loops
The syntax for a **nested ***for*** loop in C#** is as follows

```csharp
for (init; condition; increment) 
{
  // Outer Loop 
  for (init; condition; increment) 
  { 
    // Inner Loop

    // Statements
  }
}
```
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
[code-task title="Triangle of Stars" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
# Solution: Triangle of Stars
[code-task title="Triangle of Stars" executionStrategy="csharp-dot-net-core-code" requiresInput]
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