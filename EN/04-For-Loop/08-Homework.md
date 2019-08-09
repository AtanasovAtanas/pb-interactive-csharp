[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Number Sequence
[code-task title="Number Sequence" taskId="p-01" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n representing the count of numbers to read next
* Finds the max and the min numbers
* Prints them on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|Max number: 304|
|10|Min number: 0|
|304||
|0||
|0||
|50||
[/slide]

[slide]
# Solution: Number Sequence
[code-task title="Number Sequence" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      int min = int.MaxValue;
      int max = int.MinValue;
      for (int i = 0; i < n; i++)
      {
          int num = int.Parse(Console.ReadLine());
          if (num < min) min = num;
          if (num > max) max = num;
      }
      Console.WriteLine($"Max number: {max}");
      Console.WriteLine($"Min number: {min}");
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n representing the count of numbers to read next
* Finds the max and the min numbers
* Prints them on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|Max number: 304|
|10|Min number: 0|
|304||
|0||
|0||
|50||
[/slide]

[slide]
# Problem: Power Of Numbers
[code-task title="Power Of Numbers" taskId="p-02" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads p – the power and n – the number
* Prints the result of n powered by p
* Don't use Math.Pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|32|
|2||
|4|81|
|3||
[/slide]

[slide]
# Solution: Power Of Numbers
[code-task title="Power Of Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int p = int.Parse(Console.ReadLine());
      int n = int.Parse(Console.ReadLine());
      int result = 1;
      for(int i = 0; i < p; i++)
      {
        result = result * n;
      }
      Console.WriteLine(result);
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads p – the power and n – the number
* Prints the result of n powered by p
* Don't use Math.Pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|32|
|2||
|4|81|
|3||
[/slide]

[slide]
# Problem: Equal Pairs
[code-task title="Equal Pairs" taskId="p-03" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads number n and n pairs of numbers
* Prints "Yes, value=\{sum\}", if the sum of all pairs is the same
* Otherwise, prints "No, maxdiff=\{diff\}"
* diff is the max difference in the sum between two pairs
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|Yes, value=-1|
|-1||
|0||
|0||
|-1||
[/slide]

[slide]
# Solution: Equal Pairs
[code-task title="Equal Pairs" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      int prevSum = 0;
      int maxDiff = 0;
      bool areEqual = true;
      
      for (int i = 0; i < n; i++)
      {
        int a = int.Parse(Console.ReadLine());
        int b = int.Parse(Console.ReadLine());

        if (i > 0)
        {
            if (maxDiff < Math.Abs(prevSum - a - b))
            {
              maxDiff = Math.Abs(prevSum - a - b);
            }
            
            if (areEqual && a + b != prevSum) 
            {
              areEqual = false;
            }
        }

        prevSum = a + b;
      }

      if (areEqual)
      {
          Console.WriteLine($"Yes, value={prevSum}");
      }
      else
      {
          Console.WriteLine($"No, maxdiff={maxDiff}");
      }
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads number n and n pairs of numbers
* Prints "Yes, value={sum}", if the sum of all pairs is the same
* Otherwise, prints "No, maxdiff={diff}"
* diff is the max difference in the sum between two pairs
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|Yes, value=-1|
|-1||
|0||
|0||
|-1||
[/slide]

[slide]
# Problem: Bigger Number
[code-task title="Bigger Number" taskId="p-04" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n - number representing amount of input numbers
* Reads n numbers
* Finds and prints the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|90|
|40||
|90||
|50||
|3|-40|
|-40||
|-90||
|-50||
[/slide]

[slide]
# Solution: Bigger Number
[code-task title="Bigger Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      int maxNumber = int.MinValue;
      for (int i = 1; i <= n; i++)
      {
        int number = int.Parse(Console.ReadLine());
        if (number > maxNumber)
        {
            maxNumber = number;
        }
      }
      
      Console.WriteLine(maxNumber);
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers
* Finds and prints the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|90|
|40||
|90||
|50||
|3|-40|
|-40||
|-90||
|-50||
[/slide]

[slide]
# Problem: Zig Zag Sum
[code-task title="Zig Zag Sum" taskId="p-05" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n - number representing amount of input numbers
* Reads n numbers 
* For every even line adds the number to the result
* For every odd line subtracts the number from the result
* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|-30|
|10||
|20||
[/slide]

[slide]
# Solution: Zig Zag Sum
[code-task title="Zig Zag Sum" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      int sum = 0;
      for (int i = 1; i <= n; i++)
      {
        int m = int.Parse(Console.ReadLine());
        if (i % 2 == 0) sum += m;
        else sum -= m;
      }
      Console.WriteLine(sum);
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers 
* For every even line adds the number to the result
* For every odd line subtracts the number from the result
* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|-30|
|10||
|20||
[/slide]

[slide]
# Problem: Divide Without Remainder
[code-task title="Divide Without Remainder" taskId="p-06" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n and n numbers
* Finds in percentage how many of them can divide without remainder at 2, 3 and 4
* Prints percentages p1, p2 and p3, formatted to the second digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|33.33%|
|3|100.00%|
|6|0.00%|
|9||
[/slide]

[slide]
# Solution: Divide Without Remainder
[code-task title="Divide Without Remainder" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      double p1 = 0.0;
      double p2 = 0.0;
      double p3 = 0.0;
      for (int i = 0; i < n; i++)
      {
        int num = int.Parse(Console.ReadLine());
        if (num % 2 == 0) p1++;
        if (num % 3 == 0) p2++;
        if (num % 4 == 0) p3++;
      }
      var resultP1 = (p1 / n) * 100;
      var resultP2 = (p2 / n) * 100;
      var resultP3 = (p3 / n) * 100;
      
      Console.WriteLine($"{resultP1:F2}%");
      Console.WriteLine($"{resultP2:F2}%");
      Console.WriteLine($"{resultP3:F2}%");
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n and n numbers
* Finds in percentage how many of them can divide without remainder at 2, 3 and 4
* Prints percentages p1, p2 and p3, formatted to the second digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|33.33%|
|3|100.00%|
|6|0.00%|
|9||
[/slide]

[slide]
# Problem: Vowel Sum
[code-task title="Vowel Sum" taskId="p-07" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n - the count of characters:
* If character is vowel adds its value to the result

    |character|a|e|i|o|u|
    |---------|-|-|-|-|-|
    |value|1|2|3|4|5|

* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|1|
|a||
|g||
|2|8|
|i||
|u||
[/slide]

[slide]
# Solution: Vowel Sum
[code-task title="Vowel Sum" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      int vowelSum = 0;
      for (int i = 0; i < n; i++)
      {
        char letter = char.Parse(Console.ReadLine());
        switch (letter)
        {
            case 'a':
              vowelSum += 1;
              break;
            case 'e':
              vowelSum += 2;
              break;
            case 'i':
              vowelSum += 3;
              break;
            case 'o':
              vowelSum += 4;
              break;
            case 'u':
              vowelSum += 5;
              break;
        }
      }
      Console.WriteLine(vowelSum);
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - the count of characters:
* If character is vowel adds its value to the result

    |character|a|e|i|o|u|
    |---------|-|-|-|-|-|
    |value|1|2|3|4|5|

* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2<br>a<br>g|1|
|2<br>i<br>u|8|
[/slide]

[slide]
# Problem: Rollercoaster
[code-task title="Rollercoaster" taskId="p-08" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads rollercoaster places, minimum age, count of people on the queue and age for each person
* If all places are taken, prints - "The rollercoaster departures"
* In other case, prints "Waiting..."
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|1|
|a||
|g||
|2|8|
|i||
|u||
[/slide]

[slide]
# Solution: Rollercoaster
[code-task title="Rollercoaster" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int rollercoasterPlaces = int.Parse(Console.ReadLine());
      int minAge = int.Parse(Console.ReadLine());
      int peopleCount = int.Parse(Console.ReadLine());
      int validPeopleCount = 0;
      for (int i = 0; i < peopleCount; i++) {
      int personAge = int.Parse(Console.ReadLine());
      if (personAge >= minAge 
          && rollercoasterPlaces > validPeopleCount)
          validPeopleCount++;
      } 

      if (rollercoasterPlaces == validPeopleCount)
      {
          Console.WriteLine("The rollercoaster departures");
      }
      else
      {
          Console.WriteLine("Waiting...");
      }
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads rollercoaster places, minimum age, count of people on the queue and age for each person
* If all places are taken, prints - "The rollercoaster departures"
* In other case, prints "Waiting..."
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1<br>10<br>1<br>15|The rollercoaster departures|
[/slide]

[slide]
# Problem: Multiply
[code-task title="Multiply" taskId="p-09" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads n 
* Prints n's multiples in the format "\{n\} x \{i\} = \{result\}"
* Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2 x 1 = 2|
||2 x 2 = 4|
||2 x 3 = 6|
||2 x 4 = 8|
||2 x 5 = 10|
||2 x 6 = 12|
||2 x 7 = 14|
||2 x 8 = 16|
||2 x 9 = 18|
||2 x 10 = 20|
[/slide]

[slide]
# Solution: Multiply
[code-task title="Multiply" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      for (int i = 1; i <= 10; i++)
      {
        int result = n * i;
        Console.WriteLine($"{n} x {i} = {result}");
      }
  }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads n 
* Prints n's multiples in the format "{n} x {i} = {result}"
* Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2 x 1 = 2|
||2 x 2 = 4|
||2 x 3 = 6|
||2 x 4 = 8|
||2 x 5 = 10|
||2 x 6 = 12|
||2 x 7 = 14|
||2 x 8 = 16|
||2 x 9 = 18|
||2 x 10 = 20|
[/slide]