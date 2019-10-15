# While or For Loop?

[slide]
# Video

[vimeo-video videoId="343930298" startTimeInSeconds="2153" endTimeInSeconds="2819" /]

[/slide]

[slide]
# While or For Loop?

`while` and `for` loops both **repeat** a block of **code**.

But there are different situations when writing code that require either the first loop, or the other.

When you know **exactly how many times** you want to loop through a block of code, use the `for` loop.
```cs live
for (int i = 0; i <= 5; i++)
{
    Console.WriteLine(i);
}
```

It is usually appropriate for loops in which the initialization and increment are single statements and logically related. 

It is more compact than `while` and it keeps the loop control statements together in one place.

But, there could be many **complex** problems where number of iterations depend upon a certain **condition** and can't be predicated beforehand. 

That means we don't know in advance **how many times** to repeat a loop.

In those situation it is better to use `while` loop.
```cs live
string command = Console.ReadLine();
int number = int.Parse(Console.ReadLine());
while (command != "End")
{
    switch (command)
    {
        case "Add":
            number += 1;
            break;
        case "Subtract":
            number -= 1;
            break;
    }

    command = Console.ReadLine();
}

Console.WriteLine(number);
```
[/slide]

[slide]
# Problem: Odd Number
[code-task title="Odd Number" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads numbers from the console until it gets an **odd number**
* Prints the **odd** number
# Example
## Input
- 2
- 4
- 8
- 3
## Output
- 3
[/task-description]
[tests]
[test]
[input]
2
4
8
5
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
# Solution: Odd Number
[code-task title="Odd Number" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        int number = int.Parse(Console.ReadLine());

        while (number % 2 == 0)
        {
            number = int.Parse(Console.ReadLine());
        }

        Console.WriteLine(number);
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program, which:

* Reads numbers from the console until it gets an **odd number**
* Prints the **odd** number
# Example
## Input
- 2
- 4
- 8
- 3
## Output
- 3
[/task-description]
[tests]
[test]
[input]
2
4
8
5
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
# Problem: Number Manipulator
[code-task title="Number Manipulator" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a number from the console
* Reads the following commands:
* **Add** - Аdds 1 to the number
* **Subtract** - Subtracts 1 from the number
* **END** -  Prints the number and stops the program
# Example
## Input
- 5
- Add
- END
## Output
- 6
[/task-description]
[tests]
[test]
[input]
4
Add
END
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
4
Subtract
END
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
4
Add
Add
Subtract
END
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
# Solution: Number Manipulator
[code-task title="Number Manipulator" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        int number = int.Parse(Console.ReadLine());
        string command = Console.ReadLine();

        while (command != "END")
        {
            switch (command)
            {
                case "Add":
                    number++;
                    break;
                case "Subtract":
                    number--;
                    break;
            }

            command = Console.ReadLine();
        }

        Console.WriteLine(number);
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program, which:

* Reads a number from the console
* Reads the following commands:
* **Add** - Аdds 1 to the number
* **Subtract** - Subtracts 1 from the number
* **END** -  Prints the number and stops the program
# Example
## Input
- 5
- Add
- END
## Output
- 6
[/task-description]
[tests]
[test]
[input]
4
Add
END
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
4
Subtract
END
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
4
Add
Add
Subtract
END
[/input]
[output]
5
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]