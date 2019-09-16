[slide]
# Problem: Trapezoid Area
[code-task title="Trapezoid Areq" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program that reads **three** numbers **b1**, **b2** and **h** and calculates the **area** of trapezoid with **bases b1 and b2** and **height h**. 

The formula for calculating **area** of a trapezoid is **((b1 + b2) / 2) * h**.

For example if we have a trapezoid with bases 8 and 13 and height 7, it will have area (8 + 13) \* 7 / 2 = 73.50

# Input

Read **three** numbers from the console:
- bases - b1 and b2 - integers in range \[1...1000\]
- height - h - integer in range \[1...1000\]

# Output

Print on the console a single number - the **area** of the trapezoid, formatted to the **second** decimal point

# Example
| **Input** | | **Output** |
| --- | --- | --- |
| 8 | | 73.50 |
| 13 | | |
| 7 | | |
[/task-description]
[tests]
[test]
[input]
8
13
7
[/input]
[output]
73.50
[/output]
[/test]
[test]
[input]
4
6
8
[/input]
[output]
40.00
[/output]
[/test]
[test]
[input]
100
200
300
[/input]
[output]
45000.00
[/output]
[/test]
[test]
[input]
3
4
5
[/input]
[output]
17.50
[/output]
[/test]
[test]
[input]
8
13
7
[/input]
[output]
73.50
[/output]
[/test]
[test]
[input]
1.2
2.5
3.7
[/input]
[output]
6.85
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]