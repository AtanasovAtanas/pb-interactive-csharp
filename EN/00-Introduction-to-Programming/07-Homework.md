[slide]
# Homework
[/slide]

[slide]
# Problem: Print "Hello C#"
[code-task title="Print Hello C#" executionStrategy="csharp-dot-net-core-code"]
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
Write a C# program, which:

Prints "Hello C#" on the console
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Print "Hello C#"
[code-task title="Print Hello C#" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine("Hello C#");
  }
}
```
[/code-editor]
[task-description]
Write a C# program, which:

Prints "Hello C#" on the console
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Problem: Calculate and Print 5 * 5
[code-task title="Calculate and Print 5 * 5" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a C# program, which:

* Calculates the value of 5 * 5
* Prints the result
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Calculate and Print 5 * 5
[code-task title="Calculate and Print 5 * 5" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine(5 * 5);
  }
}
```
[/code-editor]
[task-description]
Write a C# program, which:

* Calculates the value of 5 * 5
* Prints the result
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Problem: Name and Expression
[code-task title="Name and Expression" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to print your name at the first line and calculate and print the expression 5 + 3 at the second line
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
||Maria|
||8|
||Peter|
||8|
[/slide]

[slide]
# Solution: Name and Expression
[code-task title="Name and Expression" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine("Maria");
    Console.WriteLine(5 + 3);
  }
}
```
[/code-editor]
[task-description]
Write a program to print your name at the first line and calculate and print the expression 5 + 3 at the second line
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
||Maria|
||8|
||Peter|
||8|
[/slide]

[slide]
# Problem: Calculations
[code-task title="Calculations" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which calculates and prints the value of the following expressions:

* 5 + 3 \* 2
* 4 \* (2 + 3)
* (2 + 5)  \*  (8 - 2) \/ 7
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Calculations
[code-task title="Calculations" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine(5 + 3 * 2);
    Console.WriteLine(4 * (2 + 3));
    Console.WriteLine(
      (2 + 5) * (8 - 2) / 7);
  }
}
```
[/code-editor]
[task-description]
Write a program, which calculates and prints the value of the following expressions:

* 5 + 3 \* 2
* 4 \* (2 + 3)
* (2 + 5)  \*  (8 - 2) \/ 7
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Problem: Square of 7 * 7 Stars
[code-task title="Square of 7 * 7 Stars" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Prints a square of 7 * 7 stars like this:
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Square of 7 * 7 Stars
[code-task title="Square of 7 * 7 Stars" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

Prints a square of 7 * 7 stars like this:
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
[/task-description]
[code-io /]
[/code-task]
[/slide]
