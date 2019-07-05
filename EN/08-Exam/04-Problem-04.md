[slide]
# Problem 04
## Description
The weather is getting warmer and tourists are going hiking high in the mountains, where there is still snow. That's why they have to buy equipment.

Your task is to write a program that calculates the price of the equipment and whether the budget will be enough or not. 

Keep in mind that the shop has the following offer: Every third product is half price.

# Input
From the console you receive:
- First line – budget – real number in the range [1.00… 100000.00]
- After that a sequence of two lines (until you receive the command "Stop" or when there is a request for a purchase which exceeds the budget):
	- Product's name – string
	- Product's price – real number in the range [1.00… 5000.00]

## Output
Print on the console the following lines depending on the case:
- If you receive the command "Stop", on one line:
	- "You bought \{count of purchased products\} products for \{price of purchases\}$."
- If there is a purchase request, whose price exceeds the budget, on two lines:
	- "You don't have enough money!"
	- "You need \{money needed\}$!"

[code-task title="Problem-04" taskId="pb-may-pr-04" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
153.20

Backpack

25.20

Shoes

54

Sunglasses

30

Stop

## Output
You bought 3 products for 94.20$.

## Comments
The budget is 153.20$.

We buy a backpack for 25.20$ -> 128$ left

We buy shoes for 54$ -> 74$ left

We buy sunglasses for 30$ but every third purchase is half price, so the sunglasses' price is 30 / 2 = 15$ -> 59$ left.

We receive the command "Stop", we have bought 3 items and the total price is 25.20 + 54 + 15 = 94.20$

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