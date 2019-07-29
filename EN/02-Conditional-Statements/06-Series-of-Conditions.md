[slide]
# Sequence of If-Else Conditions
Sometimes we need to do a sequence of conditions before we decide what actions
our program will execute. In such cases, we can apply the construction 
if-else if ... -else in series. For this purpose, we use the following format:

```csharp
if (condition)
{
    // condition body;
}
else if (second condition)
{
    // condition body;
}
else if (third condition)
{
    // condition body;
}
…
else
{
    // else construction body;
}
```
[/slide]

[slide]
# Problem: Number 1...9
[code-task title="Number 1...9" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which prints a number as text: 

  * Read an **integer** in the range [1…100]
  * Print its value in the form of text (in English)
  * If the number is **greater** than 9 print ***"Number too big"***
[/task-description]
[tests]
[test]
[input]
7
[/input]
[output]
seven
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
Number too big!
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
two
[/output]
[/test]
[/tests]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|7|seven|
|10|Number too big|
|2|two|
[/slide]