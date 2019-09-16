[slide]
# Problem: Number Sequence
[code-task title="Number Sequance" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program that reads the **number of n integers**. Print out the **largest** and **smallest** number among the entered in the format described bellow.

# Input

- On the first line of input read the count of numbers N - integer \[1...100\]
- On next N lines - read a number - integer \[-100...100\]

# Output

"Max number: \{max number\}"

"Min number: \{min number\}"

# Example

| **Input** | | **Output** |
| --- | --- | --- |
| 5 | | Max number: 304 | 
| 10 | | Min number: 0 |
| 20 | | |
| 304 | | | 
| 0 | | | 
| 50 | | |
[/task-description]
[tests]
[test]
[input]
5
10
20
304
0
50
[/input]
[output]
Max number: 304
Min number: 0
[/output]
[/test]
[test]
[input]
6
250
5
2
0
100
1000
[/input]
[output]
Max number: 1000
Min number: 0
[/output]
[/test]
[test]
[input]
6
1
1000
200
50
20
10000
[/input]
[output]
Max number: 10000
Min number: 1
[/output]
[/test]
[test]
[input]
5
5000
50
20000
45
66
[/input]
[output]
Max number: 20000
Min number: 45
[/output]
[/test]
[test]
[input]
5
100
200
300
500
250
[/input]
[output]
Max number: 500
Min number: 100
[/output]
[/test]
[test]
[input]
4
10
-2
500
1000
[/input]
[output]
Max number: 1000
Min number: -2
[/output]
[/test]
[test]
[input]
1
-1
[/input]
[output]
Max number: -1
Min number: -1
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]