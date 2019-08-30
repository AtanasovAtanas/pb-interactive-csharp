[slide]
# While Loop
In programming the `while` **loop** is used when we want to **repeat** the execution of a certain logic while a condition is in effect. 

By **"condition"**, we understand every **expression** that returns `true` or `false`. When **the condition** is **wrong**, the while loop is **interrupted**, the program **continues** to execute the remaining code after the loop. 

The while loop looks like this:
```cs
while (condition)
{
  loop body;
}
```

In the code above example, condition is any **expression that returns a Boolean result** – `true` or `false`. 

It determines how long the loop body will be repeated and is called the `loop condition`. 

In this example the `loop body` is the programming code executed at each iteration of the loop, i.e. whenever the input condition is true.

In the while loop, first of all the Boolean expression is calculated and if it is `true` the sequence of operations in the body of the loop is executed. 

Then again the input condition is checked and if it is `true` again the body of the loop is executed. 

All this is repeated again and again **until at some point the conditional expression returns value** `false`.

# Example: Sequence of Numbers 2k+1
Write a program that prints all **numbers ≤ n** of the series: **1, 3, 7, 15, 31, …,** assuming that each next number = **previous number * 2 + 1**.

Here is how we can solve the problem:
- We create a num variable for the current number to which we assign an initial **value of 1**.
- For a loop condition, we put **the current number <= n**.
- In **the body of the loop**: we print the value of the current number and increase the current number by using the formula from the problem's description.

Here is a sample implementation of this idea:
```cs
int n = int.Parse(Console.ReadLine());
int num = 1;
while (num <= n)
{
  Console.WriteLine(num);
  num = 2 * num + 1;
}
```
[/slide]

[slide]
# Problem: Decreasing Numbers
[code-task title="Decreasing Numbers" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[tests]
[test]
[input]
5
[/input]
[output]
5
4
3
2
1
[/output]
[/test]
[/tests]
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
[code-task title="Decreasing Numbers" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[tests]
[test]
[input]
5
[/input]
[output]
5
4
3
2
1
[/output]
[/test]
[/tests]
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
[code-task title="Numbers in Range" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[tests]
[test]
[input]
-10
101
60
[/input]
[output]
60
[/output]
[/test]
[/tests]
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
[code-task title="Numbers in Range" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[tests]
[test]
[input]
-10
101
60
[/input]
[output]
60
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|-10|50|
|101||
|50||
[/slide]

[slide]
# Video

[vimeo-video videoId="343930298" startTimeInSeconds="1304" endTimeInSeconds="2152" /]

[/slide]