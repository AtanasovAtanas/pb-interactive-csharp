# Revision 

[slide]
# Video

[vimeo-video videoId="341948488" startTimeInSeconds="1007" endTimeInSeconds="1681" /]

[/slide]

[slide]
# Revision 
Before proceeding ahead, let's remind ourselves about the program concepts and techniques that we have learned in the last session.

# Nested Conditions
```cs
if (condition1)
{
    if (condition2)
        // body; 
    else
        // body;
}
```

# Complex Conditions with `&&,` `||`, `!` and `()`
```cs
if ((x == left || x == right) && y >= top && y <= bottom)
{
    Console.WriteLine(…);
}
```

# Switch-Case Conditions
```cs
switch (selector)
{
    case value1:
        construction;
        break;
    case value2:
    case value3:
        construction;
        break;
    …
    default:
        construction;
        break;
}
```
[/slide]