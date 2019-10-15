# Iterating over Characters

[slide]
# Video

[vimeo-video videoId="341948488" startTimeInSeconds="3810" endTimeInSeconds="4528" /]

[/slide]

[slide]
# ASCII Table
**ASCII** stands for American Standard Code for Information Interchange. 
 
Computers can only understand numbers, so an **ASCII** code is the numerical representation of a character such as 'a' or '@' or an action of some sort. 

This is an example part of the table:

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/04-for-loop-ascii.png"/]

And here you can check the whole **ASCII Table**: **http://www.asciitable.com**

The columns that you would most probably use for the purposes of this course are the **decimal** and **character** ones.

For example, the decimal value of the character **'a'** is **97** and the one corresponding to **'@'** is **64**.

# Iterating over Characters
One of the advantages of C# is that we have the opportunity to use a **different data type** for a loop variable:

Here is an example of how a loop can pass sequentially through some **letters** in the English alphabet:
```cs live
for (char ch = 'a'; ch <= 'd'; ch++)
{
  Console.Write(ch + " ");
}
```

The result of running the code is all letters from `a` to `d` included, printed on a single line and separated by spaces. 
[/slide]

[slide]
# Problem: Latin Letters
[code-task title="Latin Letters" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which:

* Reads **2 letters**
* Prints **all letters** in the given range **inclusive**
# Example
## Input
- a
- c
## Output
- a b c
[/task-description]
[tests]
[test]
[input]
a
c
[/input]
[output]
a b c
[/output]
[/test]
[test]
[input]
f
l
[/input]
[output]
f g h i j k l
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Latin Letters
[code-task title="Latin Letters" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        char firstLetter = char.Parse(Console.ReadLine());
        char secondLetter = char.Parse(Console.ReadLine());
        for (char i = firstLetter; i <= secondLetter; i++)
        {
            Console.Write(i + " ");
        }
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program, which:

* Reads **2 letters**
* Prints **all letters** in the given range **inclusive**
# Example
## Input
- a
- c
## Output
- a b c
[/task-description]
[tests]
[test]
[input]
a
c
[/input]
[output]
a b c
[/output]
[/test]
[test]
[input]
f
l
[/input]
[output]
f g h i j k l
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]