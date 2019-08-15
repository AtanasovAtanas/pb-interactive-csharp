[slide]
# Nested Conditions
Pretty often the program logic requires the use of ***if*** or ***if-else statements***, which are contained one inside another. 

They are called nested if or if-else statements. 

As implied by the title "nested", these are if or if-else statements that are placed inside other if or else statements.

```csharp
if (expression)
{
  if (nested expression)
    // Some code
  else
    // Some code
} 
```
Only if the first condition is true the nested one is checked

```csharp
if (expression)
{
  if (nested expression)
    // Some code
  else
    // Some code
    // Executes when the nested expression is false
}
```
# Deep nesting

Nesting of more than three conditional statements inside each other is not considered a good practice.

It should be avoided, mostly through optimization of the structure/the algorithm of the code and/or by using another type of conditional statement.

* Use up to 3 nested levels

[/slide]

[slide]
# Problem: Marketplace
[code-task title="Marketplace" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program which:

  * Reads a **product** and **day** from the console
  * Prints the **price**, formatted to 2nd digit, based on the price table below
[/task-description]
[tests]
[test]
[input]
Banana
Weekday
[/input]
[output]
2.50
[/output]
[/test]
[/tests]
[/code-task]

|Product|Weekday|Weekend| 
|-------|-------|-------|
|Banana|2.50|2.70|
|Apple|1.30|1.60|
|Kiwi|2.20|3.00|

# Sample Input and Output

|Input|Output|
|-----|------|
|Banana|2.50|
|Weekday||
[/slide]

[slide]
# Problem: Biggest Number of Three
[code-task title="Biggest Number of Three" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

  * Reads **3 numbers** from the console
  * Prints **the biggest** number
[/task-description]
[tests]
[test]
[input]
1
2
3
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
-1
-5
-9
[/input]
[output]
-1
[/output]
[/test]
[test]
[input]
1
5
3
[/input]
[output]
5
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output

|Input|Output|
|-----|------|
|1|3|
|2||
|3||
|-1|-1|
|-5||
|-9||
|1|5|
|5||
|3||
[/slide]