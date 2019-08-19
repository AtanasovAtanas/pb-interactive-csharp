[slide]
# Iterating over Characters
It is good to know that the for loops don't only work with numbers. 

We can solve the task by running a for loop that passes sequentially through all letters in the English alphabet:
```csharp
for (char ch = 'a'; ch <= 'd'; ch++)
{
  Console.Write(ch + " ");
}
```

# ASCII Table
**ASCII** stands for American Standard Code for Information Interchange. 
 
Computers can only understand numbers, so an **ASCII** code is the numerical representation of a character such as 'a' or '@' or an action of some sort. 

|Dec|Hx|Oct|Html|Chr|
|---|--|---|----|---|
|97|61|141|\&\#97;|a|
|98|62|142|\&\#98;|b|

* 'a' has the int value of 97
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
Write a program, which:

* Reads 2 letters
* Prints all letters in the given range inclusive
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
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|a b c|
|c||
|f|f g h i g k l|
|l||
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
Write a program, which:

* Reads 2 letters
* Prints all letters in the given range inclusive
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
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|a b c|
|c||
|f|f g h i g k l|
|l||
[/slide]

[slide]
# Video

[vimeo-video videoId="341948488" startTimeInSeconds="3810" endTimeInSeconds="4528" /]

[/slide]