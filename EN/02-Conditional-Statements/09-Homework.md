[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Guess the Password
[code-task title="Guess the Password" taskId="p-01" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check a password:

  * Read a string: the password guess
  * Print "Welcome" if the password guess is "s3cr3t!"
  * Print "Wrong password!" in all other cases 
[/task-description]
[tests]
[test]
[input]
s3cr3t!
[/input]
[output]
Welcome
[/output]
[/test]
[test]
[input]
qwerty
[/input]
[output]
Wrong password!
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|s3cr3t!|Welcome|
|qwerty|Wrong password!|
[/slide]

[slide]
# Solution: Guess the Password
[code-task title="Guess the Password" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string password = Console.ReadLine();
      if (password == "s3cr3t!")
      {
        Console.WriteLine("Welcome");
      }
      else
      {
        Console.WriteLine("Wrong password!");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program to check a password:

  * Read a string: the password guess
  * Print "Welcome" if the password guess is "s3cr3t!"
  * Print "Wrong password!" in all other cases 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|s3cr3t!|Welcome|
|qwerty|Wrong password!|
[/slide]

[slide]
# Problem: Boiling Water
[code-task title="Boiling Water" taskId="p-02" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which checks for hot water: 

  * Read a floating-point number: the water temperature (in °C)
  * Print "The water is boiling" if the number > 100
  * Prints "The water is not hot enough" in all other cases 
[/task-description]
[tests]
[test]
[input]
104.8
[/input]
[output]
The water is boiling
[/output]
[/test]
[test]
[input]
29
[/input]
[output]
The water is not hot enough
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|104.8|The water is boiling|
|29|The water is not hot enough|
[/slide]

[slide]
# Solution: Boiling Water
[code-task title="Boiling Water" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      double temperature = double.Parse(Console.ReadLine());
      if (temperature > 100)
      {
        Console.WriteLine("The water is boiling"); 
      }
      else
      {
        Console.WriteLine("The water is not hot enough");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program, which checks for hot water: 

  * Read a floating-point number: the water temperature (in °C)
  * Print "The water is boiling" if the number > 100
  * Prints "The water is not hot enough" in all other cases 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|104.8|The water is boiling|
|29|The water is not hot enough|
[/slide]

[slide]
# Problem: Speed Info
[code-task title="Speed Info" taskId="p-03" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check for fast / slow speed: 

  * Read the speed (a floating-point number)
  * Print "Slow" if the speed <= 30
  * Print "Fast" if the speed > 30
[/task-description]
[tests]
[test]
[input]
30
[/input]
[output]
Slow
[/output]
[/test]
[test]
[input]
60
[/input]
[output]
Fast
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|Slow|
|60|Fast|
[/slide]

[slide]
# Solution: Speed Info
[code-task title="Speed Info" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      double speed = double.Parse(Console.ReadLine());
      if (speed <= 30)
      {
        Console.WriteLine("Slow");
      }
      else
      {
        Console.WriteLine("Fast");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program to check for fast / slow speed: 

  * Read the speed (a floating-point number)
  * Print "Slow" if the speed <= 30
  * Print "Fast" if the speed > 30
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|Slow|
|60|Fast|
[/slide]

[slide]
# Problem: Area of Figures
[code-task title="Area of Figures" taskId="p-04" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to calculate the area of different figures:

  * Read a string: the figure type
  * Read a number (the size) or two numbers for rectangle (sizes)
  * Checks if the entered figure is square, rectangle or circle
  * Print the calculated area formatted to the second decimal
  * For unknown figure print "Unknown figure"
[/task-description]
[tests]
[test]
[input]
square
5
[/input]
[output]
25.00
[/output]
[/test]
[test]
[input]
rectangle
5
10
[/input]
[output]
50.00
[/output]
[/test]
[test]
[input]
cirlce
2.5
[/input]
[output]
19.63
[/output]
[/test]
[test]
[input]
figure
[/input]
[output]
Unknown figure
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|square|25.00|
|5||
[/slide]

[slide]
# Solution: Area of Figures
[code-task title="Area of Figures" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string figure = Console.ReadLine();
      double area = 0;
      if (figure == "square")
      {
        double size = double.Parse(Console.ReadLine());
        area = size * size;
        Console.WriteLine("{0:0.00}", area);
      }
      else if (figure == "rectangle")
      {
        double width = double.Parse(Console.ReadLine());
        double height = double.Parse(Console.ReadLine());
        area = width * height;
        Console.WriteLine("{0:0.00}", area);
      }
      else if (figure == "circle")
      {
        double radius = double.Parse(Console.ReadLine());
        area = Math.PI * radius * radius;
        Console.WriteLine("{0:0.00}", area);
      }
      else 
      {
        Console.WriteLine("Unknown figure");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate the area of different figures: 

  * Read a string: the figure type
  * Read a number (the size) or two numbers for rectangle (sizes)
  * Checks if the entered figure is square, rectangle or circle
  * Print the calculated area formatted to the second decimal
  * For unknown figure print "Unknown figure"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|square|25.00|
|5||
[/slide]

[slide]
# Problem: Tickets
[code-task title="Tickets" taskId="p-05" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to calculate a ticket price:

  * Read a ticket type: either student or regular
  * Print the price in the following format "$\{price\}":
    * The price should be formatted to 2nd digit after the decimal point
  * Student ticket price: 1.00
  * Regular ticket price: 1.60
  * For invalid type print "Invalid ticket type!"
[/task-description]
[tests]
[test]
[input]
student
[/input]
[output]
$1.00
[/output]
[/test]
[test]
[input]
regular
[/input]
[output]
$1.60
[/output]
[/test]
[test]
[input]
ticket
[/input]
[output]
Invalid ticket type!
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|student|$1.00|
|regular|$1.60|
[/slide]

[slide]
# Solution: Tickets
[code-task title="Tickets" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string ticketType = Console.ReadLine();
      if (ticketType == "student")
      {
        Console.WriteLine("$1.00");
      }
      else if (ticketType == "regular")
      {
        Console.WriteLine("$1.60");
      }
      else
      {
        Console.WriteLine("Invalid ticket type!");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate a ticket price:

  * Read a ticket type: either student or regular
  * Print the price in the following format "$\{price\}":
  * Student ticket price: 1.00
  * Regular ticket price: 1.60
  * For invalid type print "Invalid ticket type!"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|student|$1.00|
|regular|$1.60|
[/slide]

[slide]
# Problem: Coffee Shop
[code-task title="Coffee Shop" taskId="p-06" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to calculate the drink price in a coffee shop:

  * Read a drink: either "coffee" or "tea"
  * Read an extra: either "sugar" or "no"
  * Print the price in format "Final price: $\{price\}"
    * The price should be formatted to 2nd digit after the decimal point
  
Prices:
  * Coffee price: 1.00
  * Tea price: 0.60
  * Sugar price: 0.40
[/task-description]
[tests]
[test]
[input]
coffee
sugar
[/input]
[output]
$1.40
[/output]
[/test]
[test]
[input]
coffee
no
[/input]
[output]
$1.00
[/output]
[/test]
[test]
[input]
tea
sugar
[/input]
[output]
$1.00
[/output]
[/test]
[test]
[input]
tea
no
[/input]
[output]
$0.60
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|coffee|$1.40|
|sugar||
|tea|$0.60|
|no||
[/slide]

[slide]
# Solution: Coffee Shop
[code-task title="Coffee Shop" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      string drink = Console.ReadLine();
      string extra = Console.ReadLine();
      double price = 0;
      if (drink == "coffee")
      {
        price = 1.00;
      }
      else if (drink == "tea")
      {
        price = 0.60;
      }
      if (extra == "sugar")
      {
        price += 0.40;
      }
      Console.WriteLine($"Final price: ${price}");
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate the drink price in a coffee shop:

  * Read a drink: either "coffee" or "tea"
  * Read an extra: either "sugar" or "no"
  * Print the price in format "Final price: $\{price\}"
  
Prices:
  * Coffee price: 1.00
  * Tea price: 0.60
  * Sugar price: 0.40
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|coffee|$1.40|
|sugar||
|tea|$0.60|
|no||
[/slide]

[slide]
# Problem: Valid Triangle
[code-task title="Valid Triangle" taskId="p-07" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check if a triangle is valid by its sizes:

  * Read 3 integers: the sides of a triangle
  * Checks if each side is lesser than the sum of the other 2
    * Prints "Valid Triangle" if the above condition is met
    * Prints "Invalid Triangle" otherwise 
[/task-description]
[tests]
[test]
[input]
3
4
5
[/input]
[output]
Valid Triangle
[/output]
[/test]
[test]
[input]
5
8
3
[/input]
[output]
Invalid Triangle
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|Valid Triangle|
|4||
|5||
[/slide]

[slide]
# Solution: Valid Triangle
[code-task title="Valid Triangle" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      int a = int.Parse(Console.ReadLine());
      int b = int.Parse(Console.ReadLine());
      int c = int.Parse(Console.ReadLine());
      bool isValidTriangle = true;
      if (a + b <= c)
      {
        isValidTriangle = false;
      }
      else if (a + c <= b)
      {
        isValidTriangle = false;
      }
      else if (b + c <= a)
      {
        isValidTriangle = false;
      }

      if (isValidTriangle)
      {
        Console.WriteLine("Valid Triangle");
      }
      else
      {
        Console.WriteLine("Invalid Triangle");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program to check if a triangle is valid by its sizes:

  * Read 3 integers: the sides of a triangle
  * Checks if each side is lesser than the sum of the other 2
  * Prints "Valid Triangle" if the above condition is met
  * Prints "Invalid Triangle" otherwise 
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|Valid Triangle|
|4||
|5||
[/slide]