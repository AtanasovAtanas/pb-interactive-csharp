[slide]
# Solution: C# - Test Problem
[code-task title="Days to Minutes" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
public class StartUp
{
  public static void Main(string[] args)
  {
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
1 2 3 4 5
[/input]
[output]
1
2
3
4
5
[/output]
[/test]
[test]
[input]
1 2 3 4 5 6
[/input]
[output]
1
2
3
4
5
6
[/output]
[/test]
[input]
1 2 3 4 5 6 7
[/input]
[output]
1
2
3
4
5
6
7
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