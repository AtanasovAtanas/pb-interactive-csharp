[slide]
# Revision 
Before proceeding ahead, let's remind ourselves about the program concepts and techniques that we have learned in the last session.

## Nested Conditions
Pretty often the program logic requires the use of `if` or `if-else` statements, which are contained one inside another. 

They are called **nested** `if` or `if-else` statements. 

As implied by the title **"nested"**, these are `if` or `if-else` statements that are placed inside other `if` or `else` statements.
```cs
if (condition1)
{
    if (condition2)
    {
      // body; 
    }
    else
    {
      // body;
    }  
}
```

## Complex Conditions with &&, ||, ! and ()
```cs
if ((x == left || x == right) && y >= top && y <= bottom)
{
  Console.WriteLine(…);
}
```

### Logical AND

The logical **"AND"** (operator `&&)` means a few conditions have to be **fulfilled simultaneously**. 

The following table of truthfulness is applicable:

| a | b  | a && b |
|---|---|---|
| true | true | true |
| true | false | false |
| false | true | false |
| false | false | false |

### Logical OR
The logical **"OR"** (operator `||`) means that **at least one** among a few conditions is fulfilled. Similar to the operator `&&,` the logical **"OR"** accepts a few arguments of **bool** (conditional) type and returns `true` or `false`.

| a | b  | `a || b` |
|---|---|---|
| true | true | true |
| true | false | true |
| false | true | true |
| false | false | false |

### Logical Negation (NOT)
**Logical negation** (operator `!`) means a given condition is **not fulfilled**.

| a | !a |
|---|---|
| true | false |

The operator `!` accepts as an **argument** a bool variable and **returns** its value.

## Switch-Case Conditions
The `switch-case` condition works as a sequence of `if-else` blocks. 

Whenever the work of our program depends on the value of **one variable**, instead of making consecutive conditions with `if-else` blocks, we can use the conditional `switch` statement. 

It is being used for **choosing between a list of possibilities**. 

The statement compares a given value with defined constants and depending on the result, it takes an action.

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