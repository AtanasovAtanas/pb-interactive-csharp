[slide]
# Problem 02
## Description
You are the director of the movie "Programming is fun" and you have fixed time for shooting scenes.

You have to write a program that will help you determine whether the movie day will be enough to shoot the entire movie.

The movie day starts with preparing a location, which is 15% of the time for shooting!

The movie has a count of scenes that have to be shot for a given amount of time.

## Input
You receive 3 lines from the console:
- Time for shooting – whole number in the range [0… 1440]
- Scenes count– whole number in the range [5… 25]
- Duration of a scene – whole number in the range [20… 90]

## Output
Print one line on the console:
- If the time is enough to shoot the movie:
	- "You managed to finish the movie on time! You have \{time left\} minutes left!"
- If the time is NOT enough:
	- "Time is up! To complete the movie you need \{time needed\} minutes."

Time left must be rounded to the nearest whole number.


[code-task title="Problem-02" taskId="pb-may-pr-02" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
120

10

11

## Output
Time is up! To complete the movie you need 8 minutes.

## Comments
Preparing the location => 120 * 0.15 = 18 minutes

Time for shooting the scenes => 10 * 11 = 110

Time needed: 128 minutes

The time for shooting is 120 => we need 8 minutes more
 
[/task-description]
[code-io /]
[tests]
[test]
[input]
0
4
24
[/input]
[output]
Time is up! To complete the movie you need 96 minutes.
[/output]
[/test]
[test]
[input]
180
5
20
[/input]
[output]
You managed to finish the movie on time! You have 53 minutes left!
[/output]
[/test]
[test]
[input]
135
5
20
[/input]
[output]
You managed to finish the movie on time! You have 15 minutes left!
[/output]
[/test]
[test]
[input]
1440
25
90
[/input]
[output]
Time is up! To complete the movie you need 1026 minutes.
[/output]
[/test]
[test]
[input]
1000
25
90
[/input]
[output]
Time is up! To complete the movie you need 1400 minutes.
[/output]
[/test]
[test]
[input]
120
10
11
[/input]
[output]
Time is up! To complete the movie you need 8 minutes.
[/output]
[/test]
[test]
[input]
60
15
3
[/input]
[output]
You managed to finish the movie on time! You have 6 minutes left!
[/output]
[/test]
[test]
[input]
500
23
12
[/input]
[output]
You managed to finish the movie on time! You have 149 minutes left!
[/output]
[/test]
[test]
[input]
89
9
2
[/input]
[output]
You managed to finish the movie on time! You have 58 minutes left!
[/output]
[/test]
[test]
[input]
560
32
11
[/input]
[output]
You managed to finish the movie on time! You have 124 minutes left!
[/output]
[/test]
[/tests]
[/code-task]
[/slide]