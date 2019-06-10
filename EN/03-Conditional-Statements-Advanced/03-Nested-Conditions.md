[slide]
# Nested Conditions
An ***if-else*** statement can be nested within another ***if-else*** statement

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
Deep nesting is not recommended

* Use up to 3 nested levels

[/slide]

[slide]
# Problem: Marketplace
[code-task title="Marketplace" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[code-io /]
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
# Solution: Marketplace
[code-task title="Marketplace" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        string product = Console.ReadLine();
        string dayOfWeek = Console.ReadLine();

        if (product == "Banana")
        {
            if (dayOfWeek == "Weekday")
                Console.WriteLine("2.50");
            else
                Console.WriteLine("2.70");
        }
        else if (product == "Apple")
        {
            if (dayOfWeek == "Weekday")
            {
                Console.WriteLine("1.30");
            }
            else
            {
                Console.WriteLine("1.60");
            }
        }
        else if (product == "Kiwi")
        {
            if (dayOfWeek == "Weekday")
            {
                Console.WriteLine("2.20");
            }
            else
            {
                Console.WriteLine("3.00");
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program which:

  * Reads a **product** and **day** from the console
  * Prints the **price**, formatted to 2nd digit, based on the price table below
[/task-description]
[code-io /]
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
[code-task title="Biggest Number of Three" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
[code-io /]
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

[slide]
# Solution: Biggest Number of Three
[code-task title="Biggest Number of Three" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        int first = int.Parse(Console.ReadLine());
        int second = int.Parse(Console.ReadLine());
        int third = int.Parse(Console.ReadLine());

        if (first > second)
        {
            if (first > third)
            {
                Console.WriteLine(first);
            }
            else
            {
                Console.WriteLine(third);
            }
        }
        else
        {
            if (second > third)
            {
                Console.WriteLine(second);
            }
            else
            {
                Console.WriteLine(third);
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

  * Reads **3 numbers** from the console
  * Prints **the biggest** number
[/task-description]
[code-io /]
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
