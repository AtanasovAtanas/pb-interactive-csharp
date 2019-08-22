[slide]
# Revision

## For-Loop
We can repeat a code block using a `for` loop:
```cs
for (int i = 1; i <= 10; i += 1)
{
   Console.WriteLine(i);
}
```

We can read a sequence of `n` numbers from the console this way:
```cs
int n = int.Parse(Console.ReadLine());
for (int i = 1; i <= n; i += 1)
{
   int num = int.Parse(Console.ReadLine());
}
```

We can iterate over characters:
```cs
for (char ch = 'a'; ch <= 'z'; ch += 1)
{
   Console.WriteLine(ch);
}
```

## Increment and Decrement Operators
Increments or decrements its operand by 1.

Both operators are supported in two forms: the postfix increment operator, `x++`, `x--`, and the prefix increment operator, `++x`, `--x`.

Prefix operator means increment / decrement the value before using it, while the postfix operator means increment / decremenet the value after using it.

```cs
int i = 3;
Console.WriteLine(i);   // output: 3
Console.WriteLine(i++); // output: 3
Console.WriteLine(i);   // output: 4
```

```cs
int i = 3;
Console.WriteLine(i);   // output: 3
Console.WriteLine(++i); // output: 4
Console.WriteLine(i);   // output: 4
```
[/slide]