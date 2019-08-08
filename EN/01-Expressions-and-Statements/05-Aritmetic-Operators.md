[slide]
# Arithmetic Operators

# Arithmetic Operators: + and -
Adding numbers (operator + )
```csharp
int a = 5;
int b = 7;
int sum = a + b;
Console.WriteLine(sum); // 12 
```

Subtracting numbers (operator - )
```csharp
int a = 15;
int b = 7;
Console.WriteLine(a - b); // 8
```
[/slide]

[slide]
# Arithmetic Operators: * and /
Multiplying numbers (operator *)
```csharp
int a = 5;
int b = 7;
Console.WriteLine(a * b); // 35
```

```csharp
int a = 25;
Console.WriteLine(a / 4); // 6
Console.WriteLine(a / 4.0); // 6.25
```
[/slide]

[slide]
# Arithmetic Operators: Division Behavior in C#
Dividing numbers is done using the / operator. It works differently with integers and floating point numbers. 

When we divide two integers, an integer division is applied, and the obtained output is without its fractional part. 

When we divide two numbers and at least one of them is a float number, a floating division is 
applied, and the obtained result is a float number, just like in math.

The integer division by 0 causes an exception during runtime, but Float numbers divided by 0 
do not cause an exception and the result is +/- infinity or a special value NaN.

When **dividing integers**, the result is also an integer:
```csharp
var a = 25;
Console.WriteLine(a / 4);  // Integer result: 6
Console.WriteLine(a / 0);  // Error: division by 0
```

When **dividing floating-points**, the result is also a floating-point number and the division never fails, and works correctly with the special values +∞ and -∞:

```csharp
var a = 15;
Console.WriteLine(a / 2.0);   // Float result: 7.5
Console.WriteLine(a / 0.0);   // Result: Infinity
Console.WriteLine(-a / 0.0);  // Result: -Infinity
Console.WriteLine(0.0 / 0.0); // Result: NaN
```

When printing the values ∞ and -∞, the console output may be ?, because the console in Windows does not work correctly with Unicode and breaks most of the non-standard symbols, letters and special characters. 

The example above would most probably give the following result:
```csharp
7.5
?
-?
NaN
```
[/slide]

[slide]
# Arithmetic Operators: %
Modulo / remainder from integer division (operator **%** )
```csharp
int a = 7;
int b = 2;
Console.WriteLine(a % b);   // 1
```

```csharp
Console.WriteLine(3 % 2);   // 1
Console.WriteLine(4 % 2);   // 0
Console.WriteLine(3.5 % 1); // 0.5
```
[/slide]