[slide]
# Infinite While Loop
We call an infinite loop one that repeats infinitely the performance of its body. 

In `while` and `do-while` loops the end check is a conditional expression that always returns `true`. 

```csharp
while (true)
{
  // Commands
}
```

# Example: Infinite While Loop (Bug)
```csharp
string command = "Add";
while (command != "End") 
{
  Console.WriteLine("Executing: " + command);
}
```

In the example above, the codinition is always true because it is never changed.

# Example: Finite Loop (Bug Fixed)
```csharp
string command = "Add";
while (command != "End")
{
  Console.WriteLine("Executing: " + command);

  command = Console.ReadLine();
}
```

Here, the value of the variable `command` is changed at each iteration and the **infinite loop** is avoided. 
[/slide]