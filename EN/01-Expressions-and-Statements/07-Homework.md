[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Days to Minutes
[code-task title="Days to Minutes" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to convert from days to minutes:

  * Read a single **integer** (the **days** to be converted)
  * Convert the days to minutes (use calculations)
  * Print the **minutes**
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|2|2880|
|5|7200|
[/slide]

[slide]
# Solution: Days to Minutes
[code-task title="Days to Minutes" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int days = int.Parse(Console.ReadLine());
      int hours = days * 24;
      int minutes = hours * 60;
      Console.WriteLine(minutes);
    }
}
```
[/code-editor]
[task-description]
Write a program to convert from days to minutes:

  * Read a single **integer** (the **days** to be converted)
  * Convert the days to minutes (use calculations)
  * Print the **minutes**
[/task-description]
[code-io /]
[tests]
[test]
[input]
2
[/input]
[output]
2880
[/output]
[/test]
[test]
[input]
5
[/input]
[output]
7200
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|2|2880|
|5|7200|
[/slide]

[slide]
# Solution: Print "Hello C#"
[code-task title="Print Hello C#" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine("Hello C#");
  }
}
```
[/code-editor]
[task-description]
Write a C# program, which:

Prints "Hello C#" on the console
[/task-description]
[code-io /]
[/code-task]
[/slide]