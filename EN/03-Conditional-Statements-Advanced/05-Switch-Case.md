[slide]
# The Switch-Case Statement
Used for choosing among a list of possibilities

Alternative to an ***if-else*** statement

```csharp
switch (selector)
{
  case value1:
    statements;
    break;
  default:
    statements;
    break;
}
```
Example

```csharp
string choice = Console.ReadLine();
switch (choice)
{
  case "Y":
    Console.WriteLine("Yes");
    break;
  case "N":
    Console.WriteLine("No");
    break;
  default:
    Console.WriteLine("Invalid response");
    break;
}
```
[/slide]

[slide]
# Multiple Labels
Same logic has for more than one case

```csharp
switch (selector) {
  case value1:
  case value2:
    statements;
    break;
  default:
    statements; 
    break;
}
```

Example

```csharp
string animal = Console.ReadLine();
switch (animal) {
  case "dog":
  case "cat":
    Console.WriteLine("mammal");
    break;
  default:
    Console.WriteLine("unknown"); 
    break;
}
```
[/slide]