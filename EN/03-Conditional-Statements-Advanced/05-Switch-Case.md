[slide]
# The Switch-Case Statement
The switch-case condition works as a sequence of **if-else** blocks. 

Whenever the work of our program depends on the value of one variable, instead of making consecutive conditions with if-else blocks, we can use the conditional switch statement. 

It is being used for choosing between a list of possibilities. 

The statement compares a given value with defined constants and depending on the result, it takes an action.

 - We put the variable that we want to compare, inside the brackets after the operator switch and it is called a "selector". 
 - Here the type must be comparable (numbers, strings). 
 - Consecutively, the program starts comparing each value that is found after the case labels. 
 - Upon a match, the execution of the code from the respective place begins and continues until it reaches the operator break. 

In some programming languages (like C and C++) break might be skipped, in order to execute a code from other case construction, until it reaches another operator. 

In C# though, the presence of break is mandatory for every case that contains a program logic. When no matches are found, the default construction is being executed, if such exists.

```csharp
switch (selector)
{
  case value1:
    statements;
    break;
  case value2:
    statements;
    break;
  default:
    statements;
    break;
}
```
[/slide]

[slide]
# The default case
The default case specifies the switch section to execute if the match expression doesn't match any other case label

If a default case is not present and the match expression doesn't match any other case label, program flow falls through the switch statement

The default case can appear in any order in the switch statement, but regardless of its order in the source code, it's always evaluated last, after all case labels have been evaluated

# Example
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
In C# we can use multiple case labels, when we need to execute identical logic for different cases. 

```csharp
switch (selector)
{
    case value1:
    case value2:
      statements;
      break;
    default:
      statements; 
      break;
}
```

# Example
```csharp
string animal = Console.ReadLine();
switch (animal)
{
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

[slide]
# Video

[vimeo-video videoId="341560361" startTimeInSeconds="5248" endTimeInSeconds="6535" /]

[/slide]