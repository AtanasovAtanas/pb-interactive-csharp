[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Sum Digits
[code-task title="Sum Digits" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
* **Sums** the **digits** of a number
* Prints the sum
[/task-description]
[tests]
[test]
[input]
123456
[/input]
[output]
21
[/output]
[/test]
[test]
[input]
489451
[/input]
[output]
31
[/output]
[/test]
[test]
[input]
8498498
[/input]
[output]
50
[/output]
[/test]
[test]
[input]
000000
[/input]
[output]
0
[/output]
[/test]
[test]
[input]
5684915
[/input]
[output]
38
[/output]
[/test]
[test]
[input]
8
[/input]
[output]
8
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5634|18|
[/slide]

[slide]
# Solution: Sum Digits
[code-task title="Sum Digits" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
    int n = int.Parse(Console.ReadLine());
    int sum = 0;
    while (n > 0)
    {
      sum += n % 10;
      n /= 10;
    }
    Console.WriteLine(sum);
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* **Sums** the **digits** of a number
* Prints the sum
[/task-description]
[tests]
[test]
[input]
123456
[/input]
[output]
21
[/output]
[/test]
[test]
[input]
489451
[/input]
[output]
31
[/output]
[/test]
[test]
[input]
8498498
[/input]
[output]
50
[/output]
[/test]
[test]
[input]
000000
[/input]
[output]
0
[/output]
[/test]
[test]
[input]
5684915
[/input]
[output]
38
[/output]
[/test]
[test]
[input]
8
[/input]
[output]
8
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5634|18|
[/slide]

[slide]
# Problem: Favorite Book
[code-task title="Favorite Book" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a **book's name** from the console
* Receives names until it gets **book with the same name as the first one**
* Prints "Book found! Attempts: \{attemptsCount\}" and stops afterwards
[/task-description]
[tests]
[test]
[input]
Fav Book
Book1
Book2
Book3
Fav Book
[/input]
[output]
Book found! Attempts: 4
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Alice in Wonderland|Book Found! Attempts: 3|
|Winnie the Pooh||
|Peter Pan||
|Alice in Wonderland||
[/slide]

[slide]
# Solution: Favorite Book
[code-task title="Favorite Book" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
    string favoriteBook = Console.ReadLine();
    string book = Console.ReadLine();

    int counter = 0;
    while(book != favoriteBook)
    {
      counter += 1;
      book = Console.ReadLine();
    }

    Console.WriteLine($"Book found! Attempts: {counter}");
  }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads a **book's name** from the console
* Receives names until it gets the **same book**
* Prints **"Book found!"** and stops afterwards
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Alice in Wonderland|Book Found!|
|Winnie the Pooh||
|Peter Pan||
|Alice in Wonderland||
[/slide]

[slide]
# Problem: Min and Max
[code-task title="Min and Max" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Receives integers until **"END"**
* Prints the **biggest** and the **smallest** integer
[/task-description]
[tests]
[test]
[input]
5
10
66
456
-4
1
0
END
[/input]
[output]
Max number: 456
Min number: -4
[/output]
[/test]
[test]
[input]
3
15
56
32
7
9
END
[/input]
[output]
Max number: 56
Min number: 3
[/output]
[/test]
[test]
[input]
-34
-4
-12
-45
END
[/input]
[output]
Max number: -4
Min number: -45
[/output]
[/test]
[test]
[input]
0
1
4
5
END
[/input]
[output]
Max number: 5
Min number: 0
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|Max number: 304|
|20|Min number: 0|
|304||
|0||
|50||
|END||
[/slide]

[slide]
# Solution: Min and Max
[code-task title="Min and Max" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
    int min = int.MaxValue;
    int max = int.MinValue;
    
    string line = Console.ReadLine();

    while (line != "END")
    {
      int n = int.Parse(line);

      if (n < min)
        min = n;
      if (n > max)
        max = n;

      line = Console.ReadLine();
    }

    Console.WriteLine($"Max number: {max}");
    Console.WriteLine($"Min number: {min}");
  }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives integers until **"END"**
* Prints the **biggest** and the **smallest** integer
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|Max number: 304|
|20|Min number: 0|
|304||
|0||
|50||
|END||
[/slide]

[slide]
# Problem: Special Number
[code-task title="Special Number" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Special number is number divisible by all of its digits without remainder. 

Write a program, which: 
* Receives integer
* Prints "\{num\} is special", if the number is special
* Otherwise, prints "\{num\} is not special"
[/task-description]
[tests]
[test]
[input]
55
[/input]
[output]
55 is special
[/output]
[/test]
[test]
[input]
43
[/input]
[output]
43 is not special
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|44|44 is special|
[/slide]

[slide]
# Solution: Special Number
[code-task title="Special Number" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
    int originNumber = int.Parse(Console.ReadLine());
    int number = originNumber;
    bool isSpecial = true;

    while (number > 0)
    {
      int digit = number % 10;
      number /= 10;

      if (originNumber % digit != 0)
      {
        isSpecial = false;
        break;
      }
    }

    if (isSpecial)
    {
      Console.WriteLine($"{originNumber} is special");
    }
    else
    {
      Console.WriteLine($"{originNumber} is not special");
    }
  }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives integer
* Prints "\{num\} is special" if the number is special
* Special number is number divisible by all of its digits without remainder
* Otherwise, prints "\{num\} is not special"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|44|44 is special|
[/slide]

[slide]
# Problem: Special Bonus
[code-task title="Special Bonus" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads an integer number from the console
* Keeps reading integers until it finds the same one as the first one
* When it finds it, it increases the value of the **previous** number **before it** with 20% and prints it
[/task-description]
[tests]
[test]
[input]
20
5
10
20
[/input]
[output]
12
[/output]
[/test]
[test]
[input]
20
20
[/input]
[output]
24
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|25|36|
|20||
|30||
|25||
[/slide]

[slide]
# Solution: Special Bonus
[code-task title="Special Bonus" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
    int special = int.Parse(Console.ReadLine());
    int number = Console.ReadLine();
    int previous = number;
    
    while(true)
    {
      if(number == special)
      {
        previous += previous * 0.2;
        break;
      }

      previous = number
      number = Console.ReadLine();
    }

    Console.WriteLine(previous);
  }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads an integer number from the console
* Keeps reading integers until it finds the same one as the first one
* When it finds it, it increases the value of the **previous** number **before it** with 20% and prints it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|25|36|
|20||
|30||
|25||
[/slide]

[slide]
# Problem: Sequence 2k + 1
[code-task title="Sequence 2k + 1" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a number **n** from the console
* Prints a **sequence** of numbers, which are **<= n** and satisfy the following condition:
* Each number is equal to the previous one multiplied by **2** plus **1**
[/task-description]
[tests]
[test]
[input]
1
[/input]
[output]
1
[/output]
[/test]
[test]
[input]
7
[/input]
[output]
1
3
7
[/output]
[/test]
[test]
[input]
100
[/input]
[output]
1
3
7
15
31
63
[/output]
[/test]
[test]
[input]
511
[/input]
[output]
1
3
7
15
31
63
127
255
511
[/output]
[/test]
[test]
[input]
10000
[/input]
[output]
1
3
7
15
31
63
127
255
511
1023
2047
4095
8191
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|8|1|
||3|
||7|
[/slide]

[slide]
# Solution: Sequence 2k + 1
[code-task title="Sequence 2k + 1" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
    int n = int.Parse(Console.ReadLine());
    int k = 1;
    while(k <= n)
    {
      Console.WriteLine(k);
      k = k * 2 + 1;
    }
  }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads a number **n** from the console
* Prints a **sequence** of numbers, which are **<= n** and satisfy the following condition:
* Each number is equal to the previous one multiplied by **2** plus **1**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|8|1|
||3|
||7|
[/slide]

[slide]
# Problem: Account Balance
[code-task title="Account Balance" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Receives the amount of money for each transaction untill "END"
* Adds the money to the balance and prints: "Increase: \{money\}", format `money` to the 2nd digit after the decimal point
* After "END" calculates and prints the total balance: "Total: \{balance\}", format `balance` to the 2nd digit after the decimal point
[/task-description]
[tests]
[test]
[input]
5.50
60.23
100
END
[/input]
[output]
Increase: 5.50
Increase: 60.23
Increase: 100
Total: ‭165.73‬
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5.51|Increase: 5.51|
|69.42|Increase: 69.42|
|100|Increase: 100.00|
|END|Total: 174.93|
[/slide]

[slide]
# Solution: Account Balance
[code-task title="Account Balance" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
    int n = int.Parse(Console.ReadLine());
    double balance = 0.0;

    while(n != 0)
    {
      double amount = double.Parse(Console.ReadLine());
      balance += amount;
      Console.WriteLine($"Increase: {amount:f2}");
      n--;
    }
    
    Console.WriteLine($"Total: {balance:f2}");
  }
}
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives an integer **n** - count of transactions
* Receives the amount of money for each transaction
* Adds the money to the balance and prints: "***Increase***: \{money\} " and calculates and prints the total balance
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3||
|5.51|Increase: 5.51|
|69.42|Increase: 69.42|
|100|Increase: 100|
||Total: 174.93|
[/slide]