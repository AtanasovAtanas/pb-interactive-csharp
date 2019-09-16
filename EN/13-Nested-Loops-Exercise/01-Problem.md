[slide]
# Problem: Numbers 1...N with Step 3
[code-task title="Numbers 1...N with Step 3" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program that reads a **number n**, introduced by the user, and prints **the numbers from 1 to n in 3 (step 3)**.

# Example

| **Input** | | **Output** |
| --- | --- | --- | 
| 10 | | 1 |
| | | 4 |
| | | 7 |
| | | 10 |


| **Input** | | **Output** |
| --- | --- | --- |
| 7| | 1|
| | | 4|
| | | 7|
[/task-description]
[tests]
[test]
[input]
1
[/input]
[output]
1
[/output]
[/test]
[test]
[input]
4
[/input]
[output]
1
4
[/output]
[/test]
[test]
[input]
20
[/input]
[output]
1
4
7
10
13
16
19
[/output]
[/test]
[test]
[input]
100
[/input]
[output]
1
4
7
10
13
16
19
22
25
28
31
34
37
40
43
46
49
52
55
58
61
64
67
70
73
76
79
82
85
88
91
94
97
100
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]