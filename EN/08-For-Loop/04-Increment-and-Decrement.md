# Increment and Decrement Operators

[slide]
# Video

[vimeo-video videoId="341948488" startTimeInSeconds="1693" endTimeInSeconds="1945" /]

[/slide]

[slide]
# Increment and Decrement Operators
The unary increment operator `++` increments its operand by 1, while the unary decrement operator `--` decrements it by 1.

The increment and decrement operators are supported in two forms: 

* the postfix increment/decrement operator, `x++`/`x--` 
* the prefix increment/decrement operator, `++x`/`--x`

## Increment Operator

### Postfix Increment Operator
The result of `x++` is the value of `x` before the operation, as the following example shows:
```cs live
int i = 3;
Console.WriteLine(i);
Console.WriteLine(i++);
Console.WriteLine(i);
```

### Prefix Increment Operator
The result of `++x` is the value of `x` after the operation, as the following example shows:
```cs live
double a = 1.5;
Console.WriteLine(a);
Console.WriteLine(++a);
Console.WriteLine(a);
```

## Decrement Operator

### Postfix Decrement Operator
The result of `x--` is the value of `x` before the operation, as the following example shows:
```cs live
int i = 3;
Console.WriteLine(i);
Console.WriteLine(i--);
Console.WriteLine(i);
```

### Prefix Decrement Operator
The result of `--x` is the value of `x` after the operation, as the following example shows:
```cs live
double a = 1.5;
Console.WriteLine(a);
Console.WriteLine(--a);
Console.WriteLine(a);
```
[/slide]