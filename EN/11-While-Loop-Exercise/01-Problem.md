[slide]
# Problem: Sequence 2k+1
[code-task title="Sequance 2k+1" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program that reads a number **n** and prints **all numbers ≤ n** from the sequence: **1, 3, 7, 15, 31**, … Every next number is calculated as you **multiply the previous number by 2 and add 1**.

# Example

| **Input** | | **Output** |  
| --- | --- | --- | 
| 8 | | 1 |
| | | 3 |
| | | 7 | 


| **Input** | | **Output** |
| --- | --- | --- |
| 31 | | 1|
| | | 3|
| | | 7|
| | | 15|
| | | 31|
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
7
[/input]
[output]
1
3
7
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
1
3
7
[/output]
[/test]
[test]
[input]
100
[/input]
[output]
1
3
7
15
31
63
[/output]
[/test]
[test]
[input]
511
[/input]
[output]
1
3
7
15
31
63
127
255
511
[/output]
[/test]
[test]
[input]
10000
[/input]
[output]
1
3
7
15
31
63
127
255
511
1023
2047
4095
8191
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]