[slide]
# Problem: Equal Pairs
[code-task title="Equal Pairs" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

There are **2 \* n** - **the count** of numbers. The first and second form a **pair**, the third and fourth also, etc. Each pair has **value** - the **sum** of the component numbers. Write a program that checks **whether all couples have equal value**. Otherwise prints **the maximum difference** between **two consecutive** couples. 

If all couples have **equal** value, print "Yes, value = \{value\}" + value. Otherwise, print "No, maxdiff = \{difference\}" + the maximum difference.

# Example

| **Input** | | **Output** | | **Comments** |
| --- | --- | --- | --- | --- |
| 4 | | No, maxdiff=4 | | values = \{2, 4, 4, 0\}|
| 1 | | | | differences = \{2, 0, 4\}|
| 1 | | | | max difference = 4|
| 3 | | | | |
| 1 | | | | |
| 2 | | | | |
| 2 | | | | |
| 0 | | | | |
| 0 | | | | |
[/task-description]
[tests]
[test]
[input]
3
1
2
0
3
4
-1
[/input]
[output]
Yes, value = 3
[/output]
[/test]
[test]
[input]
2
1
2
2
2
[/input]
[output]
No, maxdiff = 1
[/output]
[/test]
[test]
[input]
4
1
1
3
1
2
2
0
0
[/input]
[output]
No, maxdiff = 4
[/output]
[/test]
[test]
[input]
1
5
5
[/input]
[output]
Yes, value = 10
[/output]
[/test]
[test]
[input]
2
-1
0
0
-1
[/input]
[output]
Yes, value = -1
[/output]
[/test]
[test]
[input]
2
-1
2
0
-1
[/input]
[output]
No, maxdiff = 2
[/output]
[/test]
[test]
[input]
7
34
-33
52
12
-32
32
23
41
7
25
34
23
124
21
[/input]
[output]
No, maxdiff = 88
[/output]
[/test]
[test]
[input]
8
5
5
70
-60
3
7
2
8
20
-10
15
-5
0
10
10
0
[/input]
[output]
Yes, value = 10
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]