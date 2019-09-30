# Expressions

[slide]
# Video

[vimeo-video videoId="341512905" startTimeInSeconds="6613" endTimeInSeconds="6784" /]

[/slide]

[slide]
# Expressions
**Expressions** are sequences of operators, literals and variables which are evaluated to a value.
  * Consist of at least one **operand**
  * Can have 1 or more **operators**

```csharp
int y = x + 5;
```
```csharp
string name = "John Doe";
```
In most of the contexts in which expressions are used, for example in statements, the expression is expected to evaluate to some value. 

* If `x` and `y` are integers, the expression `x + y` evaluates to a numeric value. Every value has an associated type.
  * For example, if x and y are both variables of type **int**, the value of the expression `x + y` is also typed as **int**.
* If the value is assigned to a variable of a different type, or if `x` and `y` are different types, they need to be converted to a certaint type.

# Numerical expressions
In programming, we can calculate numerical expressions, for example:
```csharp
int r = (150-20) / 2 + 5;
```
The standard rule for **priorities** of arithmetic operations is applied: multiplying and dividing are always done before adding and subtracting. 

In case of an expression in **brackets**, it is calculated **first**, just like in math.
[/slide]