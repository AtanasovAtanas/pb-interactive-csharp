[slide]
# Problem: Sum Numbers
[code-task title="Sum Numbers" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program that reads **n integers** and finds their **sum**.

# Input

- On the first line of input read the **count** of numbers **n**
- Of the next **n** lines one introduces a number (integer)

# Output

Print a single number -  **sum** on the console

# Example

| **Input** | | **Output** | 
| --- | --- | --- |
| 4| | 43|
| 45| | |
| -20| | |
| 7| | |
| 11| | |
[/task-description]
[tests]
[test]
[input]
2
10
20
[/input]
[output]
30
[/output]
[/test]
[test]
[input]
3
-10
-20
-30
[/input]
[output]
-60
[/output]
[/test]
[test]
[input]
4
45
-20
7
11
[/input]
[output]
43
[/output]
[/test]
[test]
[input]
1
999
[/input]
[output]
999
[/output]
[/test]
[test]
[input]
0
[/input]
[output]
0
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]