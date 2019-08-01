[slide]
# Iterating over Characters

In C#, we can iterate over characters
```csharp
for (char ch = 'a'; ch <= 'd'; ch++)
{
  Console.Write(ch + " ");
}
```

# ASCII Table

Computers can only understand numbers

* ASCII code is the numerical representation of a character

|Dec|Hx|Oct|Html|Chr|
|---|--|---|----|---|
|97|61|141|\&\#97;|a|
|98|62|142|\&\#98;|b|

* 'a' has the int value of 97
[/slide]

[slide]
# Problem: Latin Letters

[code-task title="Latin Letters" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|ac|a b c|
|c||
|fl|f g h i g k l|
|l||
[/slide]

[slide]
# Solution: Latin Letters
[code-task title="Latin Letters" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|a b c|
|c||
|f|f g h i g k l|
|l||
[/slide]