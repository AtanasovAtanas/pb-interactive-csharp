[slide]
# The break Operator
The `break` operator stops the execution of a loop at the time it is called and continues from the first line after the end of the loop.

This means that the current iteration of the loop will not be completed, accordingly, the rest of the code in the body of the loop will not be executed.

This example breaks the loop when the input is an odd number:
```csharp
while (true)
{
  int number = int.Parse(Console.ReadLine());
  
  if (number % 2 != 0)
  {
    break;
  }
}
```
[/slide]