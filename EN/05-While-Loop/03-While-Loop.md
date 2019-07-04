[slide]
# While Loop
The **`while`** statement executes a statement or a block of statements while a specified **`Boolean expression`** evaluates to **`true`**

The expression is evaluated before each execution of the loop

# Example

The following example shows the usage of the while statement

```csharp
int n = 0;
while (n < 5)
{
    Console.WriteLine(n);
    n++;
}
```
[/slide]

[slide]
# Problem: Decreasing Numbers
[code-task title="Decreasing Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a number from the console
* Prints the numbers starting from the number to 1 (**inclusive**)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|4|
||3|
||2|
||1|
[/slide]

[slide]
# Solution: Decreasing Numbers
[code-task title="Decreasing Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
      int number = int.Parse(Console.ReadLine());
      while (number >= 1)
      {
          Console.WriteLine(number);
          number--;
      }
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Prints the numbers starting from the number to 1 (**inclusive**)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|4|
||3|
||2|
||1|
[/slide]

[slide]
# Problem: Numbers in Range
[code-task title="Numbers in Range" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a **number** from the console
* Checks if the number is in the range between **1 and 100**
* If it isn't - it reads a **new one**
* If it is - **prints the number** and the program stops
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|-10|50|
|101||
|50||
[/slide]

[slide]
# Solution: Numbers in Range
[code-task title="Numbers in Range" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
      int num = int.Parse(Console.ReadLine());
      while (num < 1 || num > 100)
      {
          num = int.Parse(Console.ReadLine());
      }
      Console.WriteLine(num);
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a **number** from the console
* Checks if the number is in the range between **1 and 100**
* If it isn't - it reads a **new one**
* If it is - **prints the number** and the program stops
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|-10|50|
|101||
|50||
[/slide]