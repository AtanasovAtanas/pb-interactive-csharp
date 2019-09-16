[slide]
# Problem: Max Number
[code-task title="Max Number" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput ]
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

Write a program that takes as input **n count integers (n > 0)** and finds the **max** among them. First you read the count of numbers **n**, and after that the **numbers** - each on a **single** line.

# Example

| **Input** | | **Output** |
| --- | --- | --- |
| 3 | | 20 | 
| -10 | | | | 
| 20 | | |
| -30  | | |

| **Input** | | **Output** |
| --- | --- | --- |
| 2 | | -1 |
| -1 | | |
| -2 | | |
[/task-description]
[tests]
[test]
[input]
2
100
99
[/input]
[output]
100
[/output]
[/test]
[test]
[input]
3
-10
20
-30
[/input]
[output]
20
[/output]
[/test]
[test]
[input]
4
45
-20
7
99
[/input]
[output]
99
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
5
-1000
-2000
-3000
-4000
-5000
[/input]
[output]
-1000
[/output]
[/test]
[test]
[input]
2
-1
-2
[/input]
[output]
-1
[/output]
[/test]
[test]
[input]
5
-5000
-4000
-3000
-2000
-1000
[/input]
[output]
-1000
[/output]
[/test]
[test]
[input]
30
1
2
3
4
5
6
7
8
9
10
100
200
300
400
500
600
700
800
900
999
-100
-200
-300
-400
-500
-600
-700
-800
-900
-1000
[/input]
[output]
999
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]