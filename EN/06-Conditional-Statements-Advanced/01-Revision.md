# Revision

[slide]
# Video

[vimeo-video videoId="341560361" startTimeInSeconds="1002" endTimeInSeconds="1285" /]

[/slide]

[slide]
# Revision
Let's revise what we learned in the last lesson:
- Numbers can be **compared** by the `==`, `<`, `>`, `<=`, `>=` and `!=` operators:
```cs live
Console.WriteLine(5 <= 10);  // True
```

- Simple **if-conditions** check a condition and execute a code block if it is **true**:
```cs live
int a = 10;
if (a > 5)
{
    Console.WriteLine("The number `a` is bigger than 5");
}
```

- The **if-else construction** executes one of two blocks depending on whether a condition is **true** or **false**:
```cs live
int a = 10;
if (a > 5)
{
    Console.WriteLine("The number `a` is bigger than 5");
}
else
{
    Console.WriteLine("The number `a` is smaller or equal than 5");
}
```

- If-else constructions can be chained as **if-else-if-else sequences**:
```cs live
int a = 10;
if (a > 100)
{
    Console.WriteLine("The number `a` is bigger than 100");
}
else if (a > 20)
{
    Console.WriteLine("The number `a` is bigger than 20");
}
else
{
    Console.WriteLine("The number `a` is smaller or equal than 20");
}
```
[/slide]