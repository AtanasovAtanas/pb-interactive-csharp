[slide]
# Problem: Vowels Sum
[code-task title="Vowels Sum" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program that reads **text (string)**, entered by the user, **calculates** and **prints** the **sum** of the **values** of the **vowel** letters according to the table below:

| **Letter** | | **Value** |
| --- | --- | --- |
| a| | 1|
| e| | 2|
| i| | 3|
| o| | 4|
| u| | 5|

# Example

| **Input** | | **Output** | | **Comments** |
| --- | --- | --- | --- | --- |
| hello | | 6 | | e + o = 2 + 4 = 6 |


| **Input** | | **Output** | | **Comments** |
| --- | --- | --- | --- | --- |
| bamboo | | 9 | | a + o + o = 1 + 4 + 4 = 9 |
[/task-description]
[tests]
[test]
[input]
hello
[/input]
[output]
6
[/output]
[/test]
[test]
[input]
hi
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
bamboo
[/input]
[output]
9
[/output]
[/test]
[test]
[input]
beer
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
welcome to software university
[/input]
[output]
32
[/output]
[/test]
[test]
[input]
xxx
[/input]
[output]
0
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]