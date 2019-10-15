# Logical Expressions

[slide]
# Video

[vimeo-video videoId="341532970" startTimeInSeconds="1489" endTimeInSeconds="2018" /]

[/slide]

[slide]
# Comparison Operators
In programming, we can compare values using the following operators:

|Operators|Designation|
|---------|-----------|
| Equal to |   **==** |
| Not Equal to |   **!=** |
| Greater than |   **>** |
| Greater than or equal to |   **>=** |
| Less than |   **<** |
| Less than or equal to |   **<=** |

When compared, the result is a Boolean value `true` or `false`, depending on whether the result of the comparison is `true` or `false`.
[/slide]

[slide]
# Examples for Comparing Numbers
Examples of such an expression are as follows:
```cs live
int a = 5;
int b = 10;
Console.WriteLine(a < b);
Console.WriteLine(a > 100);
Console.WriteLine(a <= 5);
Console.WriteLine(b == 2 * a);
Console.WriteLine(a != b);
```

**Note** that when printing the `true` and `false` values in C# language, they are printed with a capital letter, respectively `True` and `False`.

You can also compare numeric expressions. 

The expressions you compare can themselves be complex expressions, as in the following example.

```cs
x / 45 * (y +17) >= Math.Sqrt(z) / (p - (x * 16))
```

The preceding complex expression includes literals, variables, and function calls. 

The expressions on both sides of the comparison operator are evaluated, and the resulting values are then compared using the `>=` comparison operator. 

If the value of the expression on the left side is greater than or equal to the value of the expression on the right, the entire expression evaluates to `true`, otherwise, it evaluates to `false`.
[/slide]

[slide]
# String Comparison
Comparing text using the equality operator(`==`).

Two string operands are equal when both of them are `null` or both string instances are of the same length and have identical characters in each character position:
```cs live
string a = "Examplе";
string b = a;
Console.WriteLine(a == b);
```

```cs live
string a = "hello";
string b = "hello";
Console.WriteLine(a == b);
Console.WriteLine(a < b);
```

A string is an object and every object has an instance, but this is a knowledge we will acquire later on throughout the course.
[/slide]