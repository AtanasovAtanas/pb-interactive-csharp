[slide]
# For Loop with Step

The step part in a for loop can either increase or decrease the value of a variable

```csharp
for (int i = 0; i < 10; i += 2)
  Console.WriteLine(i);
```
```csharp
// Always pay attention on the condition
for (int i = 10; i >= 0; i -= 2)
  Console.WriteLine(i);
```
[/slide]

[slide]
# Problem: Numbers Ending with 7
[code-task title="Numbers Ending with 7" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a number n
* Prints all numbers from 7 to n, ending with 7
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|7|
||17|
||27|
[/slide]

[slide]
# Solution: Numbers Ending with 7
[code-task title="Numbers Ending with 7" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
    int n = int.Parse(Console.ReadLine());
    for (int i = 7; i <= n; i += 10)
    {
      Console.WriteLine(i);
    }
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number n
* Prints all numbers from 7 to n, ending with 7
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|27|7<br>17<br>27|
|40|7<br>17<br>27<br>37|
[/slide]

[slide]
# Problem: Exam Countdown
[code-task title="Exam Countdown" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads an integer - count of days before an exam
* For each day prints: "{currentDay} days before the exam"
* At the end prints: "The exam has come"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|3 days before the exam<br>2 days before the exam<br>1 days before the exam<br>The exam has come|
[/slide]

[slide]
# Solution: Exam Countdown
[code-task title="Exam Countdown" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
    int days = int.Parse(Console.ReadLine());

    for (int i = days; i >= 1; i -= 1)
    {
      Console.WriteLine($"{i} days before the exam");
    }
    
    Console.WriteLine("The exam has come");
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads an integer - count of days before an exam
* For each day prints: "{currentDay} days before the exam"
* At the end prints: "The exam has come"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|3 days before the exam|
||2 days before the exam|
||1 days before the exam|
||The exam has come|
[/slide]