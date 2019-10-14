[slide]
# Revision

# While / Do-While Loops
The while / do-while loops are repeated while a **condition is true**:

```cs live
int n = 10;
int num = 1;
while (num <= n)
{
   Console.WriteLine(num++);
}
```

``` cs live
int num = 1;
int count = 0;
do
{
    count++;
    num = num * 2;
} while (num <= 10);
Console.WriteLine("2^{0} = {1}", count, num);
```

# While or For
**While** and **for** loops help to **repeat** block of **code**.

Use `for` when you know the **number of repetitions**.

Use `while` when you don't know when the **end condition** will be met.

# The break Statement
If we have to **interrupt** the loop execution, we do it with the operator `break`:
``` cs live
while (true)
{
   int n = int.Parse(Console.ReadLine());
   
   if (n % 2 == 0)
   {
      break;
   }

   Console.WriteLine("The number is not even.");
}

Console.WriteLine("Even number entered: {0}", n);
```
[/slide]

[slide]
# Video

[vimeo-video videoId="342526930" startTimeInSeconds="982" endTimeInSeconds="1520" /]

[/slide]