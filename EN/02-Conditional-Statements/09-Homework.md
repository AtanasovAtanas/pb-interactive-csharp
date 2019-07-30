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
circle
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
# Video

[vimeo-video videoId="341532970" startTimeInSeconds="8356" endTimeInSeconds="10980" /]

[/slide]