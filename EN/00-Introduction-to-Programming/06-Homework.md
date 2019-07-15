[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Print "Hello C#"
[code-task title="Print Hello C#" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
[tests]
[test]
[input]
[/input]
[output]
Hello C#
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Print "Hello C#"
[code-task title="Print Hello C#" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
[tests]
[test]
[input]
[/input]
[output]
Hello C#
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Problem: Calculate and Print 5 * 5
[code-task title="Calculate and Print 5 * 5" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
[tests]
[test]
[input]
[/input]
[output]
25
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Calculate and Print 5 * 5
[code-task title="Calculate and Print 5 * 5" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
[tests]
[test]
[input]
[/input]
[output]
25
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Problem: Name and Expression
[code-task title="Name and Expression" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
Write a program to print 'Catlyn' at the first line and calculate and print the expression 5 + 3 at the second line
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
Catlyn
8
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Name and Expression
[code-task title="Name and Expression" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine("Catlyn");
    Console.WriteLine(5 + 3);
  }
}
```
[/code-editor]
[task-description]
Write a program to print 'Catlyn' at the first line and calculate and print the expression 5 + 3 at the second line
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
Catlyn
8
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Problem: Calculations
[code-task title="Calculations" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
[tests]
[test]
[input]
[/input]
[output]
11
20
6
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Calculations
[code-task title="Calculations" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
[tests]
[test]
[input]
[/input]
[output]
11
20
6
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Problem: Square of 7 * 7 Stars
[code-task title="Square of 7 * 7 Stars" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
[tests]
[test]
[input]
[/input]
[output]
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Square of 7 * 7 Stars
[code-task title="Square of 7 * 7 Stars" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
[tests]
[test]
[input]
[/input]
[output]
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
[/output]
[/test]
[/tests]
[/code-task]
[/slide]
