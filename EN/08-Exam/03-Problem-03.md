[slide]
# Problem 03
## Description
The director of a big movie production wants to know whether the budget he has will be enough to shoot the movie. 

Help him by writing a program that calculates how much it would cost him to shoot the movie. 

The price for one shooting day depends on the season and the destination:

|   | Dubai | Sofia | London |
|---|---|---|---|
| Winter | 45 000$ | 17 000$ | 24 000$ |
| Summer | 40 000$ | 12 500$ | 20 250$ |

There are the following tax reliefs:
- If the destination is Dubai – 30% discount of the total price
- If the destination is Sofia – the price is 25% higher 

## Input
You receive 4 lines from the console:
- Movie budget – real number in the range [100 000.0… 2 000 000.0]
- Destination – string: "Dubai", "Sofia" or "London"
- Season – string: "Summer" or "Winter"
- Count days – whole number in the range [1… 40]

## Output
Print one line on the console:
- If the budget is enough: 
	- "The budget for the movie is enough! We have \{budget left\}$ left!"
- If the budget is NOT enough:
	- "The director needs \{needed sum\}$ more!"

The result must be formatted to two digits after the decimal point.

[code-task title="Problem-03" taskId="pb-may-pr-03" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
	public static void Main()
	{
		// Write your code here
	}
}
```
[/code-editor]
[task-description]
## Input
400000

Sofia

Winter

20

## Output
The director needs 25000.00$ more!

## Comments
The destination is Sofia in the season Winter => the price for a day is 17000 

20 days * 17000 = 34000$

The destination is Sofia, which means that the price is 25% higher => 34000 + 25% = 425000$

Budget 400000 - 425000 => it is not enough

We need 25000$ more

[/task-description]
[code-io /]
[tests]
[test]
[input]
2000000
Dubai
Winter
40
[/input]
[output]
The budget for the movie is enough! We have 740000.00$ left!
[/output]
[/test]
[test]
[input]
100000
Dubai
Summer
20
[/input]
[output]
The director needs 460000.00$ more!
[/output]
[/test]
[test]
[input]
450509.36
Sofia
Winter
33
[/input]
[output]
The director needs 250740.64$ more!
[/output]
[/test]
[test]
[input]
1500000
Sofia
Summer
13
[/input]
[output]
The budget for the movie is enough! We have 1296875.00$ left!
[/output]
[/test]
[test]
[input]
400000
London
Winter
9
[/input]
[output]
The budget for the movie is enough! We have 184000.00$ left!
[/output]
[/test]
[test]
[input]
1930930
London
Summer
40
[/input]
[output]
The budget for the movie is enough! We have 1120930.00$ left!
[/output]
[/test]
[test]
[input]
100000
London
Summer
5
[/input]
[output]
The director needs 1250.00$ more!
[/output]
[/test]
[test]
[input]
100000
Sofia
Winter
1
[/input]
[output]
The budget for the movie is enough! We have 78750.00$ left!
[/output]
[/test]
[test]
[input]
800000
Sofia
Winter
40
[/input]
[output]
The director needs 50000.00$ more!
[/output]
[/test]
[test]
[input]
200000
Dubai
Winter
5
[/input]
[output]
The budget for the movie is enough! We have 42500.00$ left!
[/output]
[/test]
[/tests]
[/code-task]
[/slide]