[slide]
# Increment Operator
The unary increment operator `++` increments its operand by 1.

The increment operator is supported in two forms: the postfix increment operator, `x++`, and the prefix increment operator, `++x`.

## Postfix Increment Operator
The result of `x++` is the value of `x` before the operation, as the following example shows:
```cs
int i = 3;
Console.WriteLine(i);   // output: 3
Console.WriteLine(i++); // output: 3
Console.WriteLine(i);   // output: 4
```

## Prefix Increment Operator
The result of `++x` is the value of `x` after the operation, as the following example shows:
```cs
double a = 1.5;
Console.WriteLine(a);   // output: 1.5
Console.WriteLine(++a); // output: 2.5
Console.WriteLine(a);   // output: 2.5
```
[/slide]

[slide]
# Decrement Operator

The unary decrement operator `--` decrements its operand by 1.

The decrement operator is supported in two forms: the postfix decrement operator, `x--`, and the prefix decrement operator, `--x`.

## Postfix Decrement Operator
The result of `x--` is the value of `x` before the operation, as the following example shows:
```cs
int i = 3;
Console.WriteLine(i);   // output: 3
Console.WriteLine(i--); // output: 3
Console.WriteLine(i);   // output: 2
```

## Prefix Decrement Operator
The result of `--x` is the value of `x` after the operation, as the following example shows:
```cs
double a = 1.5;
Console.WriteLine(a);   // output: 1.5
Console.WriteLine(--a); // output: 0.5
Console.WriteLine(a);   // output: 0.5
```
[/slide]