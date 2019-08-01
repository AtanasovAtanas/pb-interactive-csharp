[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Fruit or Vegetable
[code-task title="Fruit or Vegetable" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check for fruit or vegetable:

* Read a single input line: an item from the greengrocery
* Fruits: banana, apple, kiwi, cherry, lemon, grapes
* Vegetables: cucumber, pepper, carrot, onion
* Print: "vegetable", "fruit" or "unknown"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|lemon|fruit|
|carrot|vegetable|
[/slide]

[slide]
# Solution: Fruit or Vegetable
[code-task title="Fruit or Vegetable" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        string product = Console.ReadLine();
        switch (product)
        {
            case "cucumber":
            case "pepper":
            case "carrot":
                Console.WriteLine("vegetable");
                break;
            case "banana":
            case "apple":
            case "kiwi":
            case "cherry":
            case "lemon":
            case "grapes":
                Console.WriteLine("fruit");
                break;
            default:
                Console.WriteLine("unknown");
                break;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to check for fruit or vegetable:

* Read a single input line: an item from the greengrocery
* Fruits: banana, apple, kiwi, cherry, lemon, grapes
* Vegetables: cucumber, pepper, carrot, onion
* Print: "vegetable", "fruit" or "unknown"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|lemon|fruit|
|carrot|vegetable|
[/slide]

[slide]
# Problem: Day of Week
[code-task title="Day of Week" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to print the day of week as words:

* Read and integer n: the day of the week in range [1..7]
* Print the name of the day (as words, in English)
* Print "Error" if the number is not in the given range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Monday|
|8|Error|
|7|Sunday|
[/slide]

[slide]
# Solution: Day of Week
[code-task title="Day of Week" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        int day = int.Parse(Console.ReadLine());
        switch (day)
        {
            case 1:
                Console.WriteLine("Monday");
                break;
            case 2:
                Console.WriteLine("Tuesday");
                break;
            case 3:
                Console.WriteLine("Wednesday");
                break;
            case 4:
                Console.WriteLine("Thursday");
                break;
            case 5:
                Console.WriteLine("Friday");
                break;
            case 6:
                Console.WriteLine("Saturday");
                break;
            case 7:
                Console.WriteLine("Sunday");
                break;
            default:
                Console.WriteLine("Error");
                break;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to print the day of week as words:

* Read and integer n: the day of the week in range [1..7]
* Print the name of the day (as words, in English)
* Print "Error" if the number is not in the given range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Monday|
|8|Error|
|7|Sunday|
[/slide]

[slide]
# Problem: Vowel or Consonant
[code-task title="Vowel or Consonant" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to check a letter for vowel or consonant:

* Read a letter from the English alphabet
* Print either "Vowel" or "Consonant"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|Vowel|
|E|Vowel|
|b|Consonant|
[/slide]

[slide]
# Solution: Vowel or Consonant
[code-task title="Vowel or Consonant" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        char letter = char.Parse(Console.ReadLine());

        if (letter == 'A' || letter == 'a' ||
            letter == 'E' || letter == 'e' ||
            letter == 'I' || letter == 'i' ||
            letter == 'O' || letter == 'o' ||
            letter == 'U' || letter == 'u')
        {
            Console.WriteLine("Vowel");
        }
        else
        {
            Console.WriteLine("Consonant");
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to check a letter for vowel or consonant:

* Read a letter from the English alphabet
* Print either "Vowel" or "Consonant"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|Vowel|
|E|Vowel|
|b|Consonant|
[/slide]

[slide]
# Problem: Product of 3 Numbers
[code-task title="Product of 3 Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Calculate the sign of the product of 3 numbers:

* Read 3 floating-point numbers
* Print the sign of the product of the entered 3 numbers: positive, negative or zero

Try to do this without multiplying the 3 numbers

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|negative|
|3||
|-1||
|-3|positive|
|-4||
|5||
[/slide]

[slide]
# Solution: Product of 3 Numbers
[code-task title="Product of 3 Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        double n1 = double.Parse(Console.ReadLine());
        double n2 = double.Parse(Console.ReadLine());
        double n3 = double.Parse(Console.ReadLine());

        if (n1 == 0 || n2 == 0 || n3 == 0)
        {
            Console.WriteLine("zero");
        }
        else
        {
            int negativeNumbersCount = 0;
            if (n1 < 0)
            {
                negativeNumbersCount++;
            }

            if (n2 < 0)
            {
                negativeNumbersCount++;
            }

            if (n3 < 0)
            {
                negativeNumbersCount++;
            }

            if (negativeNumbersCount % 2 == 0)
            {
                Console.WriteLine("positive");
            }
            else
            {
                Console.WriteLine("negative");
            }
        }
    }
}
```
[/code-editor]
[task-description]
Calculate the sign of the product of 3 numbers:

* Read 3 floating-point numbers
* Print the sign of the product of the entered 3 numbers: positive, negative or zero

Try to do this without multiplying the 3 numbers

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|negative|
|3||
|-1||
|-3|positive|
|-4||
|5||
[/slide]

[slide]
# Problem: Sorted Numbers
[code-task title="Sorted Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which checks for sorted 3 numbers:

* Read 3 real numbers
* Print "Ascending" if the numbers are in ascending order
* Print "Descending" if the numbers are in descending order
* Print "Not sorted" in any other case

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Ascending|
|2||
|3||
|3|Not sorted|
|1||
|2||
[/slide]

[slide]
# Solution: Sorted Numbers
[code-task title="Sorted Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        double n1 = double.Parse(Console.ReadLine());
        double n2 = double.Parse(Console.ReadLine());
        double n3 = double.Parse(Console.ReadLine());

        if (n1 < n2 && n2 < n3)
        {
            Console.WriteLine("Ascending");
        }
        else if (n1 > n2 && n2 > n3)
        {
            Console.WriteLine("Descending");
        }
        else
        {
            Console.WriteLine("Not sorted");
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which checks for sorted 3 numbers:

* Read 3 real numbers
* Print "Ascending" if the numbers are in ascending order
* Print "Descending" if the numbers are in descending order
* Print "Not sorted" in any other case

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Ascending|
|2||
|3||
|3|Not sorted|
|1||
|2||
[/slide]

[slide]
# Problem: Vacation Expenses
[code-task title="Vacation Expenses" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program, which calculates vacation expenses:

* Read season, accommodation type and count of the days
* Print the total expenses, based on the price table bellow,formatted to the 2nd * digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Season|Hotel|Camping|Discount|
|-----|------|-------|--------|
|Spring|30|10|20%|
|Summer|50|30|0%|
|Autumn|20|15|30%|
|Winter|40|10|10%|
# Sample Input and Output
|Input|Output|
|-----|------|
|Winter|180.00|
|Hotel||
|5||
[/slide]

[slide]
# Solution: Vacation Expenses
[code-task title="Vacation Expenses" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        string season = Console.ReadLine();
        string accommodation = Console.ReadLine();
        int days = int.Parse(Console.ReadLine());
        double totalPrice = 0.0;

        if (season == "Spring")
        {
            if (accommodation == "Hotel")
            {
                totalPrice = days * 30 * 0.80;
            }
            else if (accommodation == "Camping")
            {
                totalPrice = days * 10 * 0.80;
            }
        }
        else if (season == "Summer")
        {
            if (accommodation == "Hotel")
            {
                totalPrice = days * 50;
            }
            else if (accommodation == "Camping")
            {
                totalPrice = days * 30;
            }
        }
        else if (season == "Autumn")
        {
            if (accommodation == "Hotel")
            {
                totalPrice = days * 20 * 0.7;
            }
            else if (accommodation == "Camping")
            {
                totalPrice = days * 15 * 0.7;
            }
        }
        else if (season == "Winter")
        {
            if (accommodation == "Hotel")
            {
                totalPrice = days * 40 * 0.9;
            }
            else if (accommodation == "Camping")
            {
                totalPrice = days * 10 * 0.9;
            }
        }

        Console.WriteLine($"{totalPrice:F2}");
    }
}
```
[/code-editor]
[task-description]
Write a program, which calculates vacation expenses:

* Read season, accommodation type and count of the days
* Print the total expenses, based on the price table bellow,formatted to the 2nd * digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Season|Hotel|Camping|Discount|
|-----|------|-------|--------|
|Spring|30|10|20%|
|Summer|50|30|0%|
|Autumn|20|15|30%|
|Winter|40|10|10%|
# Sample Input and Output
|Input|Output|
|-----|------|
|Winter|180.00|
|Hotel||
|5||
[/slide]

[slide]
# Problem: Cinema
[code-task title="Cinema" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Calculate the price for all the tickets for a cinema movie:

* Reads the type of the movie, the rows and the seats per row in the cinema
* Prints the total price for all seats formatted to the 2nd digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Type|Price|
|-----|----|
|Premiere|12.00|
|Normal|7.50|
|Discount|5.00|
# Sample Input and Output
|Input|Output|
|-----|------|
|Normal|810.00|
|12||
|9||
[/slide]

[slide]
# Solution: Cinema
[code-task title="Cinema" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        string type = Console.ReadLine();
        int rows = int.Parse(Console.ReadLine());
        int cols = int.Parse(Console.ReadLine());
        int seats = rows * cols;

        switch (type)
        {
            case "Premiere":
                Console.WriteLine("{0:f2}", seats * 12.0);
                break;
            case "Normal":
                Console.WriteLine("{0:f2}", seats * 7.50);
                break;
            case "Discount":
                Console.WriteLine("{0:f2}", seats * 5.00);
                break;
        }
    }
}
```
[/code-editor]
[task-description]
Calculate the price for all the tickets for a cinema movie:

* Reads the type of the movie, the rows and the seats per row in the cinema
* Prints the total price for all seats formatted to the 2nd digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Type|Price|
|-----|----|
|Premiere|12.00|
|Normal|7.50|
|Discount|5.00|
# Sample Input and Output
|Input|Output|
|-----|------|
|Normal|810.00|
|12||
|9||
[/slide]

[slide]
# Problem: Operations with Numbers
[code-task title="Operations with Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to apply an operator for given two numbers:

* Read two real numbers and math operator from the console
* The math operator could be: "+", "-", "/", "%" and "*"
* The output should be in the following format: "\{N1\} \{operator\} \{N2\} = \{result\}"

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|10 + 12 = 22|
|12||
|+||
[/slide]

[slide]
# Solution: Operations with Numbers
[code-task title="Operations with Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        double num1 = double.Parse(Console.ReadLine());
        double num2 = double.Parse(Console.ReadLine());
        string operation = Console.ReadLine();

        double result = 0;
        if (operation == "+")
        {
            result = num1 + num2;
        }
        else if (operation == "-")
        {
            result = num1 - num2;
        }
        else if (operation == "*")
        {
            result = num1 * num2;
        }
        else if (operation == "/")
        {
            result = num1 / num2;
        }
        else if (operation == "%")
        {
            result = num1 % num2;
        }

        Console.WriteLine("{0} {1} {2} = {3}", num1, operation, num2, result);
    }
}
```
[/code-editor]
[task-description]
Write a program to apply an operator for given two numbers:

* Read two real numbers and math operator from the console
* The math operator could be: "+", "-", "/", "%" and "*"
* The output should be in the following format: "\{N1\} \{operator\} \{N2\} = \{result\}"

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|10 + 12 = 22|
|12||
|+||
[/slide]

[slide]
# Problem: ATM
[code-task title="ATM" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to simulate an ATM withdrawal:

* Read: balance, withdraw and limit
* Print "The withdraw was successful." if the balance is enough
* Print "The daily limit was exceeded." if the limit is exceeded
* Print "Insufficient availability." if the balance isn't enough

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|420|The withdraw was successful.|
|20||
|25||
|10|The daily limit was exceeded.|
|50|Insufficient availability.|
|20||
[/slide]

[slide]
# Solution: ATM
[code-task title="ATM" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        int balance = int.Parse(Console.ReadLine());
        int withdraw = int.Parse(Console.ReadLine());
        int limit = int.Parse(Console.ReadLine());

        if (balance >= withdraw && withdraw <= limit)
        {
            Console.WriteLine("The withdraw was successful.");
        }
        else if (withdraw > limit)
        {
            Console.WriteLine("The daily limit was exceeded.");
        }
        else if (withdraw > balance)
        {
            Console.WriteLine("Insufficient availability.");
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to simulate an ATM withdrawal:

* Read: balance, withdraw and limit
* Print "The withdraw was successful." if the balance is enough
* Print "The daily limit was exceeded." if the limit is exceeded
* Print "Insufficient availability." if the balance isn't enough

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|420|The withdraw was successful.|
|20||
|25||
|10|The daily limit was exceeded.|
|50|Insufficient availability.|
|20||
[/slide]

[slide]
# Problem: Biggest of Five Numbers
[code-task title="Biggest of Five Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program to find the biggest among 5 numbers
* Read 5 integers
* Print the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|5|
|2||
|3||
|4||
|5||
|-1|-1|
|-2||
|-3||
|-4||
|-5||
[/slide]

[slide]
# Solution: Biggest of Five Numbers
[code-task title="Biggest of Five Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
        int num4 = int.Parse(Console.ReadLine());
        int num5 = int.Parse(Console.ReadLine());

        if (num1 >= num2 && num1 >= num3 && num1 >= num4 && num1 >= num5)
        {
            Console.WriteLine(num1);
        }
        else if (num2 >= num1 && num2 >= num3 && num2 >= num4 && num2 >= num5)
        {
            Console.WriteLine(num2);
        }
        else if (num3 >= num1 && num3 >= num2 && num3 >= num4 && num3 >= num5)
        {
            Console.WriteLine(num3);
        }
        else if (num4 >= num1 && num4 >= num2 && num5 >= num3 && num4 >= num5)
        {
            Console.WriteLine(num4);
        }
        else if (num5 >= num1 && num5 >= num2 && num5 >= num3 && num5 >= num4)
        {
            Console.WriteLine(num5);
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to find the biggest among 5 numbers
* Read 5 integers
* Print the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|5|
|2||
|3||
|4||
|5||
|-1|-1|
|-2||
|-3||
|-4||
|-5||
[/slide]