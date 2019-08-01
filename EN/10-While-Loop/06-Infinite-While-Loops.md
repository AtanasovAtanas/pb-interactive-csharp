[slide]
# Infinite While Loop
Repeating a block of code an **infinite number of times**

Infinite ***while*** loops are caused when the check condition is always evaluated to ***true***

```csharp
while(true)
{
  // Commands
}
```

# Example: Infinite While Loop (Bug)

```csharp
string command = "Add";
while (command != "End") // Always true (never changed)
{
  Console.WriteLine("Executing: " + command);
}
```

# Example: Finite Loop (Bug Fixed)

```csharp
string command = "Add";

while (command != "End")
{
  Console.WriteLine("Executing: " + command);

  command = Console.ReadLine();
}

```
[/slide]