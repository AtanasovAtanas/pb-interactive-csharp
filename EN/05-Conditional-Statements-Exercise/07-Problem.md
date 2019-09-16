[slide]
# Problem: Pets
[code-task title="Pets" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        // Write code here
    }
}
```
[/code-editor]
[task-description]
# Description

Write a **program** calculating the **amount of kilograms** food Martina\'s pets will eat for the time she is **on adventure** and **checks if the food is enough**. Each animal eats certain amount food per day.

# Input

Read **five** lines from the console:

- **number of days** - an integer in range \[1…5000\]
- **left food in kilograms** - an integer in range \[0…100000\]
- **food for the dog per day in kilograms** - double in range \[0.00…100.00\]
- **food for the cat per day in kilograms** - double in range \[0.00…100.00\]
- **food for the turtle per day in grams** - double in range \[0.00…10000.00\]

# Output

Print on the console a **single** line:

- If the left food **IS enough**:
  - "\{kilograms remain\} kilos of food left."

     **The result should be rounded to the nearest lower integer**
- If the left food **IS NOT enough**:
  - "\{kilograms needed\} more kilos of food are needed."
  
     **The result should be rounded to the nearest higher integer**

# Example
## Input

Days - 2

Left food in kg - 10 

Food for dog/day in kg - 1

Food for cat/day in kg - 1

Food for turtle/day in g - 1200

## Output

3 kilos of food left.

## Comments

**Food needed for:**

**dog** = 2 days \* 1 kg = **2** kg;

**cat** = 2 days \* 1 kg = **2** kg;

**turtle** = 2 days \* 1200 g = **2.4** kg;

**Total amount of food** = 2 + 2 + 2.4 = **6.4** kg;

**6.4 < 10** => 10 - 6.4 = **3.6** -> **3 kg food remain**


## Input

Days - 5

Left food in kg - 10 

Food for dog/day in kg - 2.1

Food for cat/day in kg - 0.8

Food for turtle/day in g - 321

## Ouptut

7 more kilos of food are needed.

## Comments

**Needed food for:**

**dog** = **10.5** kg;

**cat** = 5 days \* 0.8 kg = **4** kg;

**turtle** = 5 days \* 321 g = **1.605** kg;

**Total amount of food** = 10.5 + 4 + 1.605 = **16.105** ;

16.105 – 10 = 6.105 -> 7 kg of food are needed
[/task-description]
[tests]
[test]
[input]
2
10
1
1
1200
[/input]
[output]
3 kilos of food left.
[/output]
[/test]
[test]
[input]
5
10
2.1
0.8
321
[/input]
[output]
7 more kilos of food are needed.
[/output]
[/test]
[test]
[input]
2
8
1.2
0.8
342
[/input]
[output]
3 kilos of food left.
[/output]
[/test]
[test]
[input]
4
8
3.3
2.3
1345
[/input]
[output]
20 more kilos of food are needed.
[/output]
[/test]
[test]
[input]
1
50
25
24
1000
[/input]
[output]
0 kilos of food left.
[/output]
[/test]
[test]
[input]
14
20
2.5
1.5
999
[/input]
[output]
50 more kilos of food are needed.
[/output]
[/test]
[test]
[input]
49
197
100
100
0
[/input]
[output]
9603 more kilos of food are needed.
[/output]
[/test]
[test]
[input]
86
124
0
0
0
[/input]
[output]
124 kilos of food left.
[/output]
[/test]
[test]
[input]
512
2562
2
2
3405
[/input]
[output]
1230 more kilos of food are needed.
[/output]
[/test]
[test]
[input]
987
2345
1.1
0.5
1
[/input]
[output]
764 kilos of food left.
[/output]
[/test]
[test]
[input]
5000
100000
2.5
2.01
10
[/input]
[output]
77400 kilos of food left.
[/output]
[/test]
[test]
[input]
10
319
1
1
1
[/input]
[output]
298 kilos of food left.
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]