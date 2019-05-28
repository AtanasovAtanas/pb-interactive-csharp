[slide]
# Sequence of If-Else Conditions
Sometimes we need to do a sequence of conditions before we decide what actions our program will execute. In such cases, we can apply the construction if-else if ... -else in series. For this purpose, we use the following format:

```csharp
if (condition)
{
    // condition body;
}
else if (second condition)
{
    // condition body;
}
else if (third condition)
{
    // condition body;
}
…
else
{
    // else construction body;
}
```
[/slide]

[slide]
# Problem: Number 1...9
[code-task title="Number 1...9" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which prints a number as text: 

  * Read an **integer** in the range [1…100]
  * Print its value in the form of text (in English)
  * If the number is **greater** than 9 print ***"Number too big"***
[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|7|seven|
|10|Number too big|
|2|two|
[/slide]

[slide]
# Solution: Number 1...9
[code-task title="Number 1...9" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int num = int.Parse(Console.ReadLine());
      if (num == 1)
        Console.WriteLine("one");
      else if (num == 2)
        Console.WriteLine("two");
      else if (num == 3)
        Console.WriteLine("three");
      else if (num == 4)
        Console.WriteLine("four");
      else if (num == 5)
        Console.WriteLine("five");
      else if (num == 6)
        Console.WriteLine("six");
      else if (num == 7)
        Console.WriteLine("seven");
      else if (num == 8)
        Console.WriteLine("eight");
      else if (num == 9)
        Console.WriteLine("nine");
      else
      Console.WriteLine("Number too big");
    }
}
```
[/code-editor]
[task-description]
Write a program, which prints a number as text:

  * Read an **integer** in the range [1…100]
  * Print its value in the form of text (in English)
  * If the number is **greater** than 9 print ***"Number too big"***
[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output
|Input|Output|
|-----|------|
|7|seven|
|10|Number too big|
|2|two|
[/slide]
