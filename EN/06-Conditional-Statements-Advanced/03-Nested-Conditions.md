# Nested Conditions

[slide]
# Video

[vimeo-video videoId="341560361" startTimeInSeconds="1425" endTimeInSeconds="2839" /]

[/slide]

[slide]
# Nested Conditions
Pretty often the program logic requires the use of `if` or `if-else` statements, which are contained one inside another.  
They are called **nested** `if` or `if-else` statements. 

As implied by the title **"nested"**, these are `if` or `if-else` statements that are placed inside other `if` or `else` statements.

```csharp
if (condition1)
{
    if (condition2)
    {
        // body; 
    }
    else
    {
        // body;
    }
}
```

# Example: Personal Titles
Depending on **age** (decimal number and **gender** (**m** / **f**), print a personal title:
-  "Mr." – a man (gender "m") – 16 or more years old.
-  "Master" – a boy (gender "m") under 16 years.
-  "Ms." – a woman (gender "f") – 16 or more years old.
-  "Miss" – a girl (gender "f") under 16 years.

# Solution: Person Titles
We should notice that the **output** of the program **depends on a few things**. 

**First**, we have to check what is the entered **gender** and **then** check the **age**. 

Respectively, we are going to use **a few** `if-else` blocks. 

These blocks will be **nested**, meaning from **the result** of the first, we are going to **define** which one of the **others** to execute.

The diagram below illustrates the process in detail:

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/01.Personal-titles-01.jpg"/]

After reading the input data from the console, the following program logic should be executed:
```cs
int age = int.Parse(Console.ReadLine());
string char = Console.ReadLine();

if (age < 16)
{
    if (gender == "m")
    {
        Console.WriteLine("Master");
    }
    else if (gender == "f")
    {
        Console.WriteLine("Miss");
    }
}
else
{
    if (gender == "m")
    {
        Console.WriteLine("Mr.");
    }
    else if (gender == "f")
    {
        Console.WriteLine("Ms.");
    }
}
```

# Deep nesting
Nesting of **more than three conditional statements** inside each other is not considered a good practice.

It **has to be avoided**, mostly through optimization of the structure/the algorithm of the code and/or by using another type of conditional statement.
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
# Description
Write a program which:
  * Reads a **product** and **day** from the console
  * Prints the **price**, formatted to 2nd digit, based on the price table below

|Product|Weekday|Weekend| 
|-------|-------|-------|
|Banana|2.50|2.70|
|Apple|1.30|1.60|
|Kiwi|2.20|3.00|
# Example
## Input
- Banana
- Weekday
## Output
- 2.50

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
[test]
[input]
Apple
Weekend
[/input]
[output]
1.60
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]
[/slide]

[slide]
# Solution: Marketplace
[code-task title="Marketplace" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        String product = Console.ReadLine();
        String day = Console.ReadLine();

        double price = 0;

        if (product == "Banana")
        {
            if (day == "Weekday")
            {
                price = 2.50;
            }
            else
            {
                price = 2.70;
            }
        }
        else if (product == "Apple")
        {
            if (day == "Weekday")
            {
                price = 1.30;
            }
            else
            {
                price = 1.60;
            }
        }
        else if (product == "Kiwi")
        {
            if (day == "Weekday")
            {
                price = 2.20;
            }
            else
            {
                price = 3.00;
            }
        }
        Console.WriteLine("{0:F2}", price);
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program which:
  * Reads a **product** and **day** from the console
  * Prints the **price**, formatted to 2nd digit, based on the price table below

|Product|Weekday|Weekend| 
|-------|-------|-------|
|Banana|2.50|2.70|
|Apple|1.30|1.60|
|Kiwi|2.20|3.00|
# Example
## Input
- Banana
- Weekday
## Output
- 2.50
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
[test]
[input]
Apple
Weekend
[/input]
[output]
1.60
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]
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
# Description
Write a program, which:

  * Reads **3 numbers** from the console
  * Prints **the biggest** number
# Example
## Input
- 1
- 2
- 3
## Output
- 3
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
[code-io/]
[/code-task]
[/slide]


[slide]
# Solution: Biggest Number of Three
[code-task title="Biggest Number of Three" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        int num1 = int.Parse(Console.ReadLine());
        int num2 = int.Parse(Console.ReadLine());
        int num3 = int.Parse(Console.ReadLine());

        if (num1 > num2) 
        {
            if (num1 > num3) 
            {
                Console.WriteLine(num1);
            }
            else 
            {
                Console.WriteLine(num3);
            }
        }
        else if (num2 > num1)
        {
            if (num2 > num3)
            {
                Console.WriteLine(num2);
            }
            else 
            {
                Console.WriteLine(num3);
            }
        }
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program, which:

  * Reads **3 numbers** from the console
  * Prints **the biggest** number
# Example
## Input
- 1
- 2
- 3
## Output
- 3
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
[code-io/]
[/code-task]

[/slide]