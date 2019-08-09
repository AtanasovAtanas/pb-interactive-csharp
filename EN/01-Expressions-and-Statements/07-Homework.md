[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Calculate Speed
[code-task title="Calculate Speed" taskId="p-01" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program to calculate the speed by time and distance:
  * Read 2 floating-point numbers: distance and time
  * Calculate the speed needed to travel a given distance for given time
  * Print the calculated result

[/task-description]
[tests]
[test]
[input]
10.0
2.0
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
2.0
10.0
[/input]
[output]
0.2
[/output]
[/test]
[test]
[input]
4.0
5.0
[/input]
[output]
0.8
[/output]
[/test]
[test]
[input]
4.5
10.0
[/input]
[output]
0.45
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|15|7.5| 
|2|| 
[/slide]

[slide]

# Problem: Currency Converter
[code-task title="Currency Converter" taskId="p-02" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program to convert from USD to EUR:
  * Read a **floating-point number**: the **dollars** to be converted 
  * Convert dollars to euro (use fixed rate of dollars to euro: **0.88**)
  * Print the converted value in **euro**

[/task-description]
[tests]
[test]
[input]
10.0
[/input]
[output]
8.8
[/output]
[/test]
[test]
[input]
5.0
[/input]
[output]
4.4
[/output]
[/test]
[test]
[input]
25.5
[/input]
[output]
22.44
[/output]
[/test]
[test]
[input]
12.0
[/input]
[output]
10.56
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|17|14.96| 
|87|76.56|
[/slide]

[slide]
# Problem: Area of Triangle
[code-task title="Area of Triangle" taskId="p-03" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program to calculate a triangle area:

  * Read from input a side **a** and height for that side **ha**
  * Calculate the area of a triangle by the side and height
  * Print the **area**, formatted to the **2nd digit** after decimal point

[/task-description]
[tests]
[test]
[input]
12.0
2.0
[/input]
[output]
12.00
[/output]
[/test]
[test]
[input]
5.0
4.0
[/input]
[output]
10.00
[/output]
[/test]
[test]
[input]
10.5
2.5
[/input]
[output]
13.13
[/output]
[/test]
[test]
[input]
1.6
2.8
[/input]
[output]
2.24
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5|25.00 | 
|10| | 
[/slide]

[slide]
# Problem: Four Operations
[code-task title="Four Operations" taskId="p-04" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program, which:
  * **Reads** 2 real numbers from the **console**
  * Performs **4 arithmetic operations** on the obtained 2 numbers, in the following order: **+, -, *, /**
  * **Formats** and **prints** the results like this example:

[/task-description]
[tests]
[test]
[input]
10.0
5.0
[/input]
[output]
10.00 + 5.00 = 15.00
10.00 - 5.00 = 5.00
10.00 * 5.00 = 50.00
10.00 / 5.00 = 2.00
[/output]
[/test]
[test]
[input]
2.5
6.5
[/input]
[output]
2.50 + 6.50 = 9.00
2.50 - 6.50 = -4.00
2.50 * 6.50 = 16.25
2.50 / 6.50 = 0.38
[/output]
[/test]
[test]
[input]
10.5
2.5
[/input]
[output]
10.50 + 2.50 = 13.00
10.50 - 2.50 = 8.00
10.50 * 2.50 = 26.25
10.50 / 2.50 = 4.20
[/output]
[/test]
[test]
[input]
1.6
2.8
[/input]
[output]
1.60 + 2.80 = 4.40
1.60 - 2.80 = -1.20
1.60 * 2.80 = 4.48
1.60 / 2.80 = 0.57
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5|5.00 + 10.00 = 15.00| 
|10|5.00 - 10.00 = -5.00|
||5.00 * 10.00 = 50.00|
||5.00 / 10.00 = 0.50|
[/slide]


[slide]
# Problem: Days to Minutes
[code-task title="Days to Minutes" taskId="p-05" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program to convert from days to minutes:
  * Read a single **integer** (the **days** to be converted)
  * Convert the days to minutes (use calculations)
  * Print the **minutes**

[/task-description]
[tests]
[test]
[input]
6
[/input]
[output]
8640
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
14400
[/output]
[/test]
[test]
[input]
32
[/input]
[output]
46080
[/output]
[/test]
[test]
[input]
9
[/input]
[output]
12960
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|2|2880|
|5|7200|
[/slide]

[slide]
# Problem: Circle Area and Perimeter
[code-task title="Circle Area and Perimeter" taskId="p-06" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program to calculate a circle area and perimeter:
  * Read a floating-point number: the radius of a circle
  * Calculate the area and perimeter of a circle
  * Print the calculated values

[/task-description]
[tests]
[test]
[input]
12.0
[/input]
[output]
Area = 452.389342
Perimeter = 75.398224
[/output]
[/test]
[test]
[input]
10.0
[/input]
[output]
Area = 314.159265
Perimeter = 62.831853
[/output]
[/test]
[test]
[input]
5.5
[/input]
[output]
Area = 95.033178
Perimeter = 34.557519
[/output]
[/test]
[test]
[input]
9.4
[/input]
[output]
Area = 277.591127
Perimeter = 59.061942
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|7|Area = 153.938040|
||Perimeter = 43.982297|

[/slide]

[slide]
# Problem: Person Info
[code-task title="Person Info" taskId="p-07" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program, which:
  * Reads 4 lines of **strings**: first name, last name, country and town 
  * Prints information about a person in the following format: "**{firstName} {lastName} from {country} - {town}!**"

[/task-description]
[tests]
[test]
[input]
John
Smith
USA
LA
[/input]
[output]
John Smith from USA - LA!
[/output]
[/test]
[test]
[input]
Ann
Green
France
Paris
[/input]
[output]
Ann Green from France - Paris!
[/output]
[/test]
[test]
[input]
Pesho
Peshov
Bulgaria
Sofia
[/input]
[output]
Pesho Peshov from Bulgaria - Sofia!
[/output]
[/test]
[test]
[input]
A
B
C
D
[/input]
[output]
A B from C - D!
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Kelly|Kelly Smith from Ireland - Cork!|
|Smith||
|Ireland||
|Cork||
[/slide]

[slide]
# Problem: Town Info
[code-task title="Town Info" taskId="p-08" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Write a program, which:
  * Reads **3 lines** of input: **name** (string), **population** and **area** (integers)
  * Prints information about a town in the following format: "**Town {name} has population of {population} and area {area} square km.**"

[/task-description]
[tests]
[test]
[input]
Sofia
100000
13000
[/input]
[output]
Town Sofia has population of 100000 and area 13000 square km.
[/output]
[/test]
[test]
[input]
Paris
20065
1200
[/input]
[output]
Town Paris has population of 20065 and area 1200 square km.
[/output]
[/test]
[test]
[input]
London
350000
1000
[/input]
[output]
Town London has population of 350000 and area 1000 square km.
[/output]
[/test]
[test]
[input]
A
123456
789
[/input]
[output]
Town A has population of 123456 and area 789 square km.
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Berlin|Town Berlin has population of 3675000 and area 984 square km.|
|3675000||
|984||
[/slide]

[slide]
# Video

[vimeo-video videoId="341512905" startTimeInSeconds="8642" endTimeInSeconds="10930" /]

[/slide]