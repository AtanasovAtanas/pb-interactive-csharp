[slide]
# Problem 04
## Description
The weather is warming up and the clubs are launching promising offers. 

Write a program that calculates the profit of a club for the evening and whether the desired win is reached, keeping in mind the following: 

The price of a cocktail is its length name. 

If the price of an order is an odd number, there is a 25% discount on the order price.

# Input
You will receive:
- On the first line – the desired profit of the club - real number in the range [1.00... 15000.00]

A series of two rows until the command "Party!" or until the desired profit is reached:
- Name of the cocktail - string
- Number of cocktails for the order - whole number in the range [1… 50]

## Output
First, print one line on the console:

- Until the command "Party!":
	- "We need {money needed} dollars more."
- When the desired profit is reached:
	- "Target acquired."

Then print:
- "Club income - {club's profit} dollars."

The money must be formatted to the second digit after the decimal point.

[code-task title="Problem-04" taskId="pb-june-pr-04" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
# Example 
## Input
500

Bellini

6

Bamboo

7

Party!

## Output
We need 416.00 dollars more.

Club income - 84.00 dollars.

## Comments
The goal of the club is to collect 500$.

The first order is for 6 cocktails Bellini. 

The price of the cocktail is its name length - 7. 6 Cocktails of 7$ -> 42$, the last digit is 2, therefore there is no discount.

The next order is for 7 Bamboo cocktails, its price is 6$. 6 * 7-> 42$, again there is no discount.

We receive the command Party! The program stops.

The club has 42 + 42 = 84$ and the target is 500. 500 – 84 = 416$ are needed.

[/task-description]
[code-io /]
[tests]
[test]
[input]
15354
Backpack
25.20
Shoes
54
Sunglasses
30
Backpack
25.20
Shoes
54
Sunglasses
30
Sunglasses
30
Backpack
25.20
Sunglasses
30
Backpack
25.20
Stop
[/input]
[output]
You bought 10 products for 283.80$.
[/output]
[/test]
[test]
[input]
154
Backpack
25.20
Shoes
54
Sunglasses
30
Backpack
25.20
Shoes
54
[/input]
[output]
You don't have enough money!
You need 19.40$!
[/output]
[/test]
[test]
[input]
2950
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Stop
[/input]
[output]
You bought 19 products for 320.00$.
[/output]
[/test]
[test]
[input]
150
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
50
[/input]
[output]
You don't have enough money!
You need 15.00$!
[/output]
[/test]
[test]
[input]
2999
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Backpack
20
Shoes
20
Sunglasses
40
Stop
[/input]
[output]
You bought 22 products for 390.00$.
[/output]
[/test]
[test]
[input]
200
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
50
Backpack
20
Shoes
20
[/input]
[output]
You don't have enough money!
You need 5.00$!
[/output]
[/test]
[test]
[input]
2999
Backpack
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Backpack
20
Shoes
20
Sunglasses
40
Stop
[/input]
[output]
You bought 10 products for 190.00$.
[/output]
[/test]
[test]
[input]
100
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
[/input]
[output]
You don't have enough money!
You need 20.00$!
[/output]
[/test]
[test]
[input]
2999
Backpack
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Backpack
20
Shoes
20
Sunglasses
40
Backpack
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Backpack
20
Shoes
20
Sunglasses
40
Stop
[/input]
[output]
You bought 20 products for 380.00$.
[/output]
[/test]
[test]
[input]
200
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
Backpack
20
Shoes
20
Sunglasses
20
[/input]
[output]
You don't have enough money!
You need 20.00$!
[/output]
[/test]
[/tests]
[/code-task]
[/slide]