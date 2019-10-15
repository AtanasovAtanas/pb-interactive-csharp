# Arithmetic Operations

[slide]
# Video

[vimeo-video videoId="341512905" startTimeInSeconds="5968" endTimeInSeconds="6610" /]

[/slide]

[slide]
# Arithmetic Operations
Let's examine the basic **arithmetic operations** in programming. 

We can add, subtract, multiply and divide numbers using the operators `+`, `-`, `*` and `/`.

## Summing up Numbers
We can **sum** up numbers using the `+` operator:
```cs live
int a = 5;
int b = 7;
int sum = a + b;
Console.WriteLine(sum); // 12 
```

## Subtracting Numbers
**Subtracting** numbers is done using the `-` operator:
```cs live
int a = 15;
int b = 7;
Console.WriteLine(a - b); // 8
```

## Multiplying Numbers
For **multiplication** of numbers we use the `*` operator:
```cs live
int a = 5;
int b = 7;
Console.WriteLine(a * b); // 35
```

## Dividing Numbers
**Dividing** numbers is done using the `/` operator. 

It works differently with **integers** and **floating point numbers**.
* When we divide two integers, an **integer division** is applied, and the obtained output is without its fractional part. 
  * Example: `11 / 3 = 3`.
* When we divide two numbers and at least one of them is a float number, a **floating division** is applied, and the obtained result is a float number, just like in math. 
  * Example: `11 / 4.0 = 2.75`
  * When it cannot be done with exact precision, the result is being rounded, for example `11.0 / 3 = 3.66666666666667`.
* The integer **division by 0** causes an **exception** during runtime (runtime exception).
* Float numbers **divided by 0** do not cause an exception and the result is **+/- infinity** or a special value **NaN**. 
  * Example `5 / 0.0 = ∞`.

Here are a few examples with the division operator:
```cs live
var a = 25;
var i = a / 4;
Console.WriteLine(i);
var f = a / 4.0;
Console.WriteLine(f);
```

### Dividing Integers
Let's examine a few examples for **integer division** (remember that when we **divide integers** in C# the result is an **integer**):
```cs live
int a = 25;
Console.WriteLine(a / 4);
```

Dividing an integer by zero leads to an error.
``` cs live
int a = 5;
Console.WriteLine(a / 0);
```

### Dividing Floating-Point Numbers
Let's look at a few examples for **floating division**. 

When we divide floating point numbers, the result is always a **float number** and the division never fails.

It also works correctly with the special values **+∞** and **-∞**:
```cs live
int a = 15;
Console.WriteLine(a / 2.0);
Console.WriteLine(a / 0.0);
Console.WriteLine(-a / 0.0);
Console.WriteLine(0.0 / 0.0);
```

When printing the values ∞ and -∞, the console output may be `?`.

This happens because the console in Windows does not work correctly with Unicode and breaks most of the non-standard symbols, letters and special characters.

### Remainder
The remainder operator `%` computes the remainder after dividing its left-hand operand by its right-hand operand.
```cs live
int a = 7;
int b = 2;
Console.WriteLine(a % b);
Console.WriteLine(3.5 % 1);
```
It is useful if we want to check whether a number is **even** or **odd**.

If the remainder when dividing by 2 is equal to 0, then the number is even, otherwise it is odd.

See the following example: 
```cs live
Console.WriteLine(3 % 2);
Console.WriteLine(4 % 2);
```
[/slide]