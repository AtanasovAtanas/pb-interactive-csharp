# Revision

[slide]
# Video

[vimeo-video videoId="343930298" startTimeInSeconds="975" endTimeInSeconds="1195" /]

[/slide]

[slide]
# Revision

## For-Loop
We can repeat a code block using a `for` loop:
```cs live
for (int i = 1; i <= 10; i += 1)
{
   Console.WriteLine(i);
}
```

We can read a sequence of `n` numbers from the console this way:
```cs live
int n = int.Parse(Console.ReadLine());
int sum = 0;

for (int i = 1; i <= n; i += 1)
{
   int num = int.Parse(Console.ReadLine());
   sum += num;
}

Console.WriteLine(sum);
```

We can iterate over characters:
```cs live
for (char ch = 'a'; ch <= 'z'; ch++)
{
   Console.WriteLine(ch);
}
```

## Increment and Decrement Operators
Increments or decrements its operand by 1.

Both operators are supported in two forms: the postfix increment operator, `x++`, `x--`, and the prefix increment operator, `++x`, `--x`.

Prefix operator means increment / decrement the value before using it, while the postfix operator means increment / decremenet the value after using it.

```cs live
int i = 3;
Console.WriteLine(i);   // output: 3
Console.WriteLine(i++); // output: 3
Console.WriteLine(i);   // output: 4
```

```cs live
int i = 3;
Console.WriteLine(i);   // output: 3
Console.WriteLine(++i); // output: 4
Console.WriteLine(i);   // output: 4
```
[/slide]