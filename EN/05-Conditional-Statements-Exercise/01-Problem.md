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
# Description

Write a program that reads an **integer** from the console and print if it is **even** or **odd**.

# Example

| **Input** | | **Output** |
| --- | --- | --- |
| 2 | | even |


| **Input** | | **Output** |
| --- | --- | --- |
| 25 | | odd |
[/task-description]
[tests]
[test]
[input]
3
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
even
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
[test]
[input]
1000
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
1007
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
1024
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
1
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
33333333
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
-1
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
-2
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
223156
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
123
[/input]
[output]
odd
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]