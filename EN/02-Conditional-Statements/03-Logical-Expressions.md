[slide]
# Comparison Operators
|Operators|Designation|
|---------|-----------|
| Equal to |   == |
| Not Equal to |   != |
| Greater than |   > |
| Greater than or equal to |   >= |
| Less than |   < |
| Less than or equal to |   <= |
[/slide]

[slide]
# Value Comparison
In programming we can **compare** values

  * The result of the logical expressions is either ***true*** or ***false***

Comparison operators can be used to construct expressions that compare the values
of numeric variables. These expressions return a Boolean value based on whether
the comparison is true or false. Examples of such an expression are as follows.

```csharp
int a = 5;
int b = 10;
Console.WriteLine(a < b);      // true
Console.WriteLine(a > 100);    // false
Console.WriteLine(a <= 5);     // true
Console.WriteLine(b == 2 * a); // true
Console.WriteLine(a != b);     // true
```
You can also compare numeric expressions. The expressions you compare can themselves
be complex expressions, as in the following example.
```csharp
x / 45 * (y +17) >= Math.Sqrt(z) / (p - (x * 16))
```
The preceding complex expression includes literals, variables, and function calls. 
The expressions on both sides of the comparison operator are evaluated, and the resulting
values are then compared using the >= comparison operator. If the value of the expression
on the left side is greater than or equal to the value of the expression on the right, the
entire expression evaluates to True; otherwise, it evaluates to False.

[/slide]

[slide]
# String Comparison
Comparing text using the equality operator(**==**)

Two string operands are equal when both of them are **null** or both string instances are of 
the same length and have identical characters in each character position:
```csharp
string a = "Examplе";
string b = a;
Console.WriteLine(a == b); // true
```
```csharp
string a = "hello";
string b = "hello";
Console.WriteLine(a == b); // true
Console.WriteLine(a < b); // error
```
A string is an object and every object has an instance, but this is a knowledge we will
acquire later on throughout the course.
[/slide]