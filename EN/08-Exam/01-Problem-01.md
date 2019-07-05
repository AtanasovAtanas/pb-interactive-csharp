[slide]
# Problem 01
## Description
You have been hired by "SoftUni Studios" to write a program that calculates the potential profit of movie ticket sales. 

The projection of the film takes a predetermined number of days, with a certain number of tickets sold each day. 

The price for 1 ticket is determined by the studio. 

There is a percent of the total profit that the cinema obtains for broadcasting the production. 

## Input
From the console you receive 5 lines:
- Name of the movie - string
- Days count - whole number in the range [1… 90]
- Tickets count  - whole number in the range [100… 100000]
- Ticket price - real number in the range [5.0… 25.0]
- Cinema profit percent - whole number in the range [5... 35]

## Output
Print on the console the profit from the sales in the following format:
- "The profit from the movie \{name of the movie\} is \{studio's profit\}$"
The profit must be formatted to two digits after the decimal point.

[code-task title="Problem-01" taskId="pb-may-pr-01" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
The Programmer

20

500

7.50

7

## Output
The profit from the movie The Programmer is 69750.00$

## Comments 
Price of tickets for a day => 500 * 7.50 = 3750$

Total profit => 20 * 3750 = 75000$

Percent of the profit for the cinema 

75000 * 7 / 100 = 5250$

Profit from the movie = 75000 - 5250 = 69750$

[/task-description]
[code-io /]
[tests]
[test]
[input]
Sofia Day
1
100
5
5
[/input]
[output]
The profit from the movie Sofia Day is 475.00$
[/output]
[/test]
[test]
[input]
Bulgarian Story
90
100000
25
35
[/input]
[output]
The profit from the movie Bulgarian Story is 146250000.00$
[/output]
[/test]
[test]
[input]
The What
45
50000
15.94
12
[/input]
[output]
The profit from the movie The What is 31561200.00$
[/output]
[/test]
[test]
[input]
Three Dogs
87
86899
13.89
6
[/input]
[output]
The profit from the movie Three Dogs is 98710677.06$
[/output]
[/test]
[test]
[input]
Profit
2
234
11.2
34
[/input]
[output]
The profit from the movie Profit is 3459.46$
[/output]
[/test]
[test]
[input]
HA HA
11
11111
11.11
11
[/input]
[output]
The profit from the movie HA HA is 1208509.03$
[/output]
[/test]
[test]
[input]
The programmer
20
500
7.50
7
[/input]
[output]
The profit from the movie The programmer is 69750.00$
[/output]
[/test]
[test]
[input]
Python Basics
40
34785
10.45
14
[/input]
[output]
The profit from the movie Python Basics is 12504511.80$
[/output]
[/test]
[test]
[input]
The jungle
22
20500
9.37
30
[/input]
[output]
The profit from the movie The jungle is 2958109.00$
[/output]
[/test]
[test]
[input]
Heavy Metal
39
120
12.90
17
[/input]
[output]
The profit from the movie Heavy Metal is 50108.76$
[/output]
[/test]
[/tests]
[/code-task]
[/slide]