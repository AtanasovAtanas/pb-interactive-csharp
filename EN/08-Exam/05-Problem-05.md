[slide]
# Problem 05
## Description
Write a program, which shows the movie with the highest rating, the one one with the lowest and the average rating of all the movies  that she wants to watch.  

## Input
First, you read one line from the console:
- Count of movies, which Dessie wants to watch – a whole number in the range [1…20] 

For each movie you will read two separate lines:
- Name of movie – a text 
- Movie rating – a real number in the range [1.00…10.00]

## Output
Print three lines in the following format:
- "\{name of the top rated movie\} is with highest rating: \{top movie rating\}"
- "\{name of movie with lowest rating\} is with lowest rating: \{lowest movie ratng\}"
- "Average rating: \{the average rating of all movies\}"

The top, the lowest and the average rating must be formatted one digit after the decimal separator.

[code-task title="Problem-05" taskId="pb-may-pr-05" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
5

A Star is Born

7.8

Creed 2

7.3

Mary Poppins

7.2

Vice

7.2

Captain Marvel

7.1

## Output
A Star is Born is with highest rating: 7.8

Captain Marvel is with lowest rating: 7.1

Average rating: 7.3

## Comments
5 chosen movies

The movie with highest rating is:

A Star is Born with rating 7.8

The movie with lowest rating is:

Captain Marvel with rating 7.1

The average rating is:

(7.8 + 7.3 + 7.2 + 7.2 + 7.1) / 5 = 36.5 / 5 = 7.32 ~ 7.3

[/task-description]
[code-io /]
[tests]
[test]
[input]
6
Green Mile
8.7
Avengers
8.5
Gifted
7.6
Star Wars
7.9
Firday 13th
7.4
The Favorite
7.1
[/input]
[output]
Green Mile is with highest rating: 8.7
The Favorite is with lowest rating: 7.1
Average rating: 7.9
[/output]
[/test]
[test]
[input]
4
The Choice
8.2
Dear John
7.5
The Godfather
8.9
Notebook
8.1
[/input]
[output]
The Godfather is with highest rating: 8.9
Dear John is with lowest rating: 7.5
Average rating: 8.2
[/output]
[/test]
[test]
[input]
3
The Shawshank Redemption
9.2
Forrest Gump
8.7
Gladiator
8.5
[/input]
[output]
The Shawshank Redemption is with highest rating: 9.2
Gladiator is with lowest rating: 8.5
Average rating: 8.8
[/output]
[/test]
[test]
[input]
7
Coco
8.3
Scarface
9.0
Jurassic World
8.4
12 Years a Slave
8.4
Harry Potter
8.5
Rocky
7.4
Beautiful Mind
7.9
[/input]
[output]
Scarface is with highest rating: 9.0
Rocky is with lowest rating: 7.4
Average rating: 8.3
[/output]
[/test]
[test]
[input]
2
Passengers
9.3
A Walk to Remember
7.5
[/input]
[output]
Passengers is with highest rating: 9.3
A Walk to Remember is with lowest rating: 7.5
Average rating: 8.4
[/output]
[/test]
[test]
[input]
20
The Choice
8.2
Dear John
7.5
The Godfather
8.9
Notebook
8.1
The Shawshank Redemption
9.2
Forrest Gump
8.7
Gladiator
8.5
Coco
8.3
Scarface
9.0
Jurassic World
8.4
12 Years a Slave
8.4
Harry Potter
8.5
Rocky
7.4
Beautiful Mind
7.9
Passengers
9.3
A Walk to Remember
7.5
A Star is Born
9.8
Creed 2
7.3
Mary Poppins
7.2
Vice
6.9
[/input]
[output]
A Star is Born is with highest rating: 9.8
Vice is with lowest rating: 6.9
Average rating: 8.3
[/output]
[/test]
[/tests]
[/code-task]
[/slide]