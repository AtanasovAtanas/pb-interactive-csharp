# If-Else Conditions

[slide]
# Video

[vimeo-video videoId="341532970" startTimeInSeconds="2478" endTimeInSeconds="3566" /]

[/slide]

[slide]
# If-Else Conditions
The `if` construction may also contain an `else` clause to give a specific action in case the Boolean expression (which is set at the beginning `if (bool expression)` ) returns a negative result (`false`). 

Built this way, **the conditional statement** is called `if-else` and its behavior is as follows: 
* if the result of the condition is positive (`true`) – we perform some actions
* when it is negative (`false`) – others. 

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/02-usecase-if-else-statement.png"/]

The format of the construction is:
```csharp
if (condition)
{
  // condition body;
}
else
{
  // else construction body;
}
```

If condition is `false`, the else-statement runs.

Because a condition can’t be simultaneously `true` and `false`, the then-statement and the else-statement of an `if-else` statement can **never both run**. 

After the then-statement or the `else`-statement runs, control is transferred to the next statement after the `if` statement.

In an `if` statement that doesn’t include an else statement, if condition is `true`, the then-statement runs. 

If condition is `false`, control is transferred to the next statement after the if statement.

Both the then-statement and the else-statement can consist of a single statement or multiple statements that are enclosed in braces `{ }`. 

For a single statement, the braces are optional but recommended.

The statement or statements in the then-statement and the else-statement can be of any kind, including another if statement nested inside the original if statement.

# Example: Weather
This is an extended version of the example from the previous slide.

As you can see now we have another case, which will be executed when the condition in the `if` statement turns out **false**.
```cs
string weather = Console.ReadLine();

if (weather == "rainy")
{
    Console.WriteLine("Take an umbrella!");
}
else
{
    Console.WriteLine("Leave your umbrella at home!")
}
```
[/slide]

[slide]
# Block of Code
When we have **only one command** in the body of the **if construction**, we can **skip the curly brackets**, indicating the conditional operator body. 

When we want to execute **block of code** (group of commands), curly brackets are **required**. 

In case we drop them, **only the first line** after the **if clause** will be executed.

Here is an example where dropping curly braces leads to confusion:
```cs live
string color = "red";
if (color == "red") 
  Console.WriteLine("tomato");
else
  Console.WriteLine("banana");
Console.WriteLine("lemon"); 
```

With curly braces:
```cs live
string color = "red";
if (color == "red")
{
  Console.WriteLine("tomato");
  Console.WriteLine("strawberry"); 
}
else
{
  Console.WriteLine("banana");
  Console.WriteLine("lemon");
}
```
[/slide]

[slide]
# Problem: Even or Odd
[code-task title="Even or Odd" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which checks if a number is **even** or **odd**

  * If it's even, print "**even**"
  * If it's odd, print "**odd**"
# Example
## Input
- 4
## Output
- even
## Input
- 7
## Output
- odd
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
7
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
0
[/input]
[output]
even
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Even or Odd
[code-task title="Even or Odd" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        double number = double.Parse(Console.ReadLine());

        if (number % 2 == 0)
        {
            Console.WriteLine("even");
        }
        else
        {
           Console.WriteLine("odd");
        }
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program, which checks if a number is **even** or **odd**

  * If it's even, print "**even**"
  * If it's odd, print "**odd**"
# Example
## Input
- 4
## Output
- even
## Input
- 7
## Output
- odd
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
7
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
0
[/input]
[output]
even
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Problem: Greater Numbers
[code-task title="Greater Number" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which finds the greater of two numbers:

  * Read two **integers**
  * Find the greater number
  * Print `"Greater number: "` + the **greater** number
# Example
## Input
- 4
- 8
## Output
- Greater number: 8

[/task-description]
[tests]
[test]
[input]
4
8
[/input]
[output]
Greater number: 8
[/output]
[/test]
[test]
[input]
7
3
[/input]
[output]
Greater number: 7
[/output]
[/test]
[test]
[input]
1
2
[/input]
[output]
Greater number: 2
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]


[slide]
# Solution: Greater Numbers
[code-task title="Greater Number" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
      int number1 = int.Parse(Console.ReadLine());
      int number2 = int.Parse(Console.ReadLine());

      if (number1 > number2)
      {
          Console.WriteLine("Greater number: " + number1);
      }
      else if (number2 > number1)
      {
          Console.WriteLine("Greater number: " + number2);
      }
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program, which finds the greater of two numbers:

  * Read two **integers**
  * Find the greater number
  * Print `"Greater number: "` + the **greater** number
# Example
## Input
- 4
- 8
## Output
- Greater number: 8
[/task-description]
[tests]
[test]
[input]
4
8
[/input]
[output]
Greater number: 8
[/output]
[/test]
[test]
[input]
7
3
[/input]
[output]
Greater number: 7
[/output]
[/test]
[test]
[input]
1
2
[/input]
[output]
Greater number: 2
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]
[/slide]