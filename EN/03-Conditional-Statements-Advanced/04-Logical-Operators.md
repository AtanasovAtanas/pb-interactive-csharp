[slide]
# Logical Operators
Logical Operators are used to perform the logical operation between two operands like **AND**, **OR** and **NOT** based on our requirements.

The Logical Operators will **always work with Boolean expressions** (**true** or **false**) and return **Boolean values**.

The logical operators are:
  * AND (**&&**) - **returns true if both operands are true**
  * OR (**\| \|**) - **returns true if any one operand is true**
  * Logical negation (**!**) - **returns the reverse of logical state**
    * Brackets **()** change the order

| Operand1 | Operand2 | And | Or |
|---|---|---|---|
| true | true | true | true |
| true | false | false | true |
| false | true | false | true |
| false | false | false | false |

If you observe above table, **if any one operand value become false, then the logical AND operator will return false**, same way **the logical OR operator will return true, if any one operand value become true**
[/slide]

[slide]
# Logical AND Operator
In some tasks we have to make many checks at once. 

But what happens when in order to execute some code more conditions have to be executed and we don't want to make a negation (else) for each one of them? 

The option with nested if blocks is valid, but the code would look very unordered and for sure – hard to read and maintain.

The logical ***AND*** (operator **&&**) means a few conditions have to be fulfilled simultaneously.

# How does it work?
The && operator accepts a couple of Boolean (conditional) statements, which have a true or false value, and returns one bool statement as a result. 

Using it instead of a couple of nested if blocks, makes the code more readable, ordered and easy to maintain. 

But how does it work, when we put a few conditions one after another? As we saw above, the logical ***AND*** returns **true**, only when it accepts as arguments statements with value true. 

Respectively, when we have a sequence of arguments, the logical ***AND*** checks either until one of the arguments is over, or until it meets an argument with value **false**.

Example:
```csharp
bool a = true;
bool b = true;
bool c = false;
bool d = true;
bool result = a && b && c && d;
// false (as d is not being checked)
```

The program will run in the following way: 
 - It starts the check form **a**, reads it and accepts that it has a **true** value, after which it checks **b**. 
 - After it has accepted that **a** and **b** return true, it checks the next argument. It gets to **c** and sees that the variable has a **false** value. 
 - After the program accepts that the argument **c** has a **false** value, it calculates the expression before **c**, independent of what the value of **d** is. 
 - That is why the evaluation of **d** is being skipped and the whole expression is calculated as **false**.
[/slide]

[slide]
# Logical OR Operator
The logical ***OR*** (operator **||**) means that at least one among a few conditions is fulfilled. 

Similar to the operator **&&**, the logical ***OR*** accepts a few arguments of bool (conditional) type and returns true or false. 

We can easily guess that we obtain a value true every time when at least one of the arguments has a true value. 

| Operand | Not |
|---|---|
| true | false |
| false | true |

# How does it work?
We have already learned what the logical ***OR*** represents. But how is it actually being achieved? 

Just like with the logical "AND", the program checks from left to right the arguments that are given. 

In order to obtain **true** from the expression, it is necessary for just one argument to have a **true** value. 

Respectively, the checking continues until an argument with such value is met or until the arguments are over.

Here is one example of the **||** operator in action:

```csharp
bool a = false;
bool b = true;
bool c = false;
bool d = true;
bool result = a || b || c || d;
// true (as c and d are not being checked)
```

The programs checks **a**, accepts that it has a value **false** and continues. 

Reaching **b**, it understands that it has a **true** value and the whole expression is calculated as **true**, without having to check **c** or **d**, because their values wouldn't change the result of the expression.

[/slide]

[slide]
# Logical NOT Operator
Logical negation (operator **!**) means a given condition is not fulfilled.

The operator **!** accepts as an argument a bool variable and returns its value.

**The NOT operator will always return the reverse value of operand** like **if operand value true, then the Logical NOT operator will return false and vice versa**

[/slide]

[slide]
# Problem: Bonus Points
[code-task title="Bonus Points" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
Write a program that applies bonus to given points
  * If points are between 0 and 3, adds 5
  * If points are between 4 and 6, adds 15
  * If points are between 7 and 9, adds 20
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
19
[/output]
[/test]
[test]
[input]
8
[/input]
[output]
28
[/output]
[/test]
[test]
[input]
1
[/input]
[output]
6
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]

[slide]
# Solution: Bonus Points
[code-task title="Bonus Points" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
    int points = int.Parse(Console.ReadLine());

    if (points >= 0 && points <= 3)
    {
      points += 5;
    }
    else if (points >= 4 && points <= 6)
    {
      points += 15;
    }
    else if (points >= 7 && points <= 9)
    {
      points += 20;
    }

    Console.WriteLine(points);
  }
}
```
[/code-editor]
[task-description]
Write a program that applies bonus to given points
  * If points are between 0 and 3, adds 5
  * If points are between 4 and 6, adds 15
  * If points are between 7 and 9, adds 20
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
19
[/output]
[/test]
[test]
[input]
8
[/input]
[output]
28
[/output]
[/test]
[test]
[input]
1
[/input]
[output]
6
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]

[slide]
# Problem: Food or Drink
[code-task title="Food or Drink" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
  * Reads single line and print "***drink***", "***food***" or "***unknown***"
  * Foods: curry, noodles, sushi, spaghetti 
  * Drinks: tea, water, coffee
  * Everything else is unknown
[/task-description]
[tests]
[test]
[input]
curry
[/input]
[output]
food
[/output]
[/test]
[test]
[input]
tea
[/input]
[output]
drink
[/output]
[/test]
[test]
[input]
something
[/input]
[output]
unknown
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|curry|food|
|water|drink|
|flower|unknown|
[/slide]

[slide]
# Solution: Food or Drink
[code-task title="Food or Drink" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
    string item = Console.ReadLine();

    if (item == "curry" || item == "noodles" || input == "sushi" || input == "spaghetti")
    {
      Console.WriteLine("food");
    }
    else if (item == "tea" || item == "water" || item == "coffee")
    {
      Console.WriteLine("drink");
    }
    else
    {
      Console.WriteLine("unknown");
    }
}
```
[/code-editor]
[task-description]
Write a program, which:
  * Reads single line and print "***drink***", "***food***" or "***unknown***"
  * Foods: curry, noodles, sushi, spaghetti 
  * Drinks: tea, water, coffee
  * Everything else is unknown
[/task-description]
[tests]
[test]
[input]
curry
[/input]
[output]
food
[/output]
[/test]
[test]
[input]
tea
[/input]
[output]
drink
[/output]
[/test]
[test]
[input]
something
[/input]
[output]
unknown
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|curry|food|
|water|drink|
|flower|unknown|
[/slide]