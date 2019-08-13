[slide]
# If...else Statement
In an if-else statement, **`if`** condition evaluates to **`true`**, the then-statement runs. 

```csharp
if (condition)
{
  // then-statement
  // Commands to be executed if the condition is true
}
else
{
  // else-statement
  // Commands to be executed if the condition is false
}
```

If condition is `false`, the else-statement runs.

Because a condition can’t be simultaneously `true` and `false`, the then-statement and the else-statement of an `if-else` statement can **never both run**. 

After the then-statement or the `else`-statement runs, control is transferred to the next statement after the `if` statement.

In an `if` statement that doesn’t include an else statement, if condition is `true`, the then-statement runs. 

If condition is `false`, control is transferred to the next statement after the if statement.

Both the then-statement and the else-statement can consist of a single statement or multiple statements that are enclosed in braces `{ }`. 

For a single statement, the braces are optional but recommended.

The statement or statements in the then-statement and the else-statement can be of any kind, including another if statement nested inside the original if statement.
[/slide]

[slide]
# Block of Code
The curly brackets `{ }` introduce a **block** (a group of commands).

In case the `if` statement does **not** have curly brackets, only the code on the **next line** will be executed.

```csharp
string color = "red";
if (color == "red") 
  Console.WriteLine("tomato");
else
  Console.WriteLine("banana");
Console.WriteLine("lemon"); /* <- Always executed */
```
```csharp
string color = "red";
if (color == "red")
{
  // Block of 2 commands
  Console.WriteLine("tomato");
  Console.WriteLine("strawberry"); 
}
else
{
  // Block of 2 commands
  Console.WriteLine("banana");
  Console.WriteLine("lemon");
}
```
[/slide]

[slide]
# Problem: Even or Odd
[code-task title="Even or Odd" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which checks if a number is **even** or **odd**

  * If it's even, print "**even**"
  * If it's odd, print "**odd**"
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
7
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
0
[/input]
[output]
even
[/output]
[/test]
[/tests]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|4|even|
|7|odd|
|0|even|
[/slide]

[slide]
# Problem: Greater Numbers
[code-task title="Greater Number" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which finds the greater of two numbers:

  * Read two **integers**
  * Find the greater number
  * Print ***"Greater number:"*** + the **greater** number
[/task-description]
[tests]
[test]
[input]
4
8
[/input]
[output]
Greater number: 8
[/output]
[/test]
[test]
[input]
7
3
[/input]
[output]
Greater number: 7
[/output]
[/test]
[test]
[input]
1
2
[/input]
[output]
Greater number: 2
[/output]
[/test]
[/tests]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|4|Greater number: 8|
|8||
[/slide]

[slide]
# Video

[vimeo-video videoId="341532970" startTimeInSeconds="2478" endTimeInSeconds="3566" /]

[/slide]