[slide]
# Homework - Python
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Welcome
[code-task title="Welcome" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Receives a single line: name
* Prints the following message: "Welcome, \{name\}"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|John|Welcome, John|
[/slide]

[slide]
# Solution: Welcome
[code-task title="Welcome" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
name = input()
print(f"Welcome, {name}")
```
[/code-editor]
[task-description]
Write a program, which:

* Receives a single line: name
* Prints the following message: "Welcome, \{name\}"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|John|Welcome, John|
[/slide]

[slide]
# Problem: Area of Triangle
[code-task title="Area of Triangle" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Create a function that receives two numbers:

* The side of a triangle - a
* The height for that side - ha
* Print the area formatted to the 2nd digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|25.00|
|10||
[/slide]

[slide]
# Solution: Area of Triangle
[code-task title="Area of Triangle" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
a = float(input())
h = float(input())
area = (a * h) / 2
print(f'{area:.2f}')
```
[/code-editor]
[task-description]
Create a function that receives two numbers:

* The side of a triangle - a
* The height for that side - ha
* Print the area formatted to the 2nd digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|25.00|
|10||
[/slide]

[slide]
# Problem: Four Operations
[code-task title="Four Operations" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 2 parameters
* Performs the 4 arithmetic operations, in the following order: +, -, *, /
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5|5 + 10 = 15| 
|10|5 - 10 = -5|
||5 * 10 = 50|
||5 / 10 = 0.5|
[/slide]

[slide]
# Solution: Four Operations
[code-task title="Four Operations" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
num1 = int(input())
num2 = int(input())
print(f'{num1} + {num2} = {num1 + num2}')
print(f'{num1} - {num2} = {num1 - num2}')
print(f'{num1} * {num2} = {num1 * num2}')
print(f'{num1} / {num2} = {num1 / num2}')
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 2 parameters
* Performs the 4 arithmetic operations, in the following order: +, -, *, /
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5|5 + 10 = 15| 
|10|5 - 10 = -5|
||5 * 10 = 50|
||5 / 10 = 0.5|
[/slide]

[slide]
# Problem: Days to Minutes
[code-task title="Days to Minutes" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single number (days)
* Converts the days to minutes 
* Prints the minutes
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|2|2880|
|5|7200|
[/slide]

[slide]
# Solution: Days to Minutes
[code-task title="Days to Minutes" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
days = int(input())
hours = days * 24
minutes = hours * 60
print(minutes)
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single number (days)
* Converts the days to minutes 
* Prints the minutes
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|2|2880|
|5|7200|
[/slide]

[slide]
# Problem: Currency Converter
[code-task title="Currency Converter" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number - the dollars to be converted 
* Converts dollars to euro (the rate of dollars to euro is 0.88)
* Prints the converted value in euro
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|17|14.96| 
|87|76.56|
[/slide]

[slide]
# Solution: Currency Converter
[code-task title="Currency Converter" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
dollars = float(input())
euros = dollars * 0.88
print(euros)
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number - the dollars to be converted 
* Converts dollars to euro (the rate of dollars to euro is 0.88)
* Prints the converted value in euro
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|17|14.96| 
|87|76.56|
[/slide]

[slide]
# Problem: Circle Area and Perimeter
[code-task title="Circle Area and Perimeter" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
import math

# Write your code here
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number - the radius of a circle
* Calculates the area and perimeter of a circle
* Prints the calculated values formatted to the 2nd decimal
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|7|Area = 153.93804002589985|
||Perimeter = 43.982297150257104|
[/slide]

[slide]
# Solution: Circle Area and Perimeter
[code-task title="Circle Area and Perimeter" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
import math

radius = float(input())
area = radius * radius * math.pi
perimeter = 2 * math.pi * radius
print(f'Area = {area}')
print(f'Perimeter = {perimeter}')
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number - the radius of a circle
* Calculates the area and perimeter of a circle
* Prints the calculated values formatted to the 2nd decimal
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output
|       Input       | Output |
|-------------------|--------|
|7|Area = 153.93804002589985|
||Perimeter = 43.982297150257104|
[/slide]

[slide]
# Problem: Inches to Centimeters
[code-task title="Inches to Centimeters" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number - the inches to be converted
* Calculates them to centimeters 
* Prints the result 
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|21|53.34| 
|71|180.34|
[/slide]

[slide]
# Solution: Inches to Centimeters
[code-task title="Inches to Centimeters" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
inches = float(input())
centimeters = inches * 2.54
print(centimeters)
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a number - the inches to be converted
* Calculates them to centimeters 
* Prints the result 
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|21|53.34 | 
|71|180.34|
[/slide]

[slide]
# Problem: Calculate Speed
[code-task title="Calculate Speed" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 2 numbers - distance and time
* Calculates the speed needed to travel a given distance for a given time
* Prints the calculated result
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|15|7.5| 
|2||
[/slide]

[slide]
# Solution: Calculate Speed
[code-task title="Calculate Speed" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
distance = float(input())
time = float(input())
speed = distance / time
print(speed)
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 2 numbers - distance and time
* Calculates the speed needed to travel a given distance for a given time
* Prints the calculated result
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|15|7.5| 
|2||
[/slide]

[slide]
# Problem: Person Info
[code-task title="Person Info" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 4 strings - first name, last name, country and town 
* Prints information about a person in the following format: "\{firstName\} \{lastName\} from \{country\} - \{town\}!"
[/task-description]
[code-io /]
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
# Solution: Person Info
[code-task title="Person Info" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
first_name = input()
last_name = input()
country = input()
town = input()
print(f'{first_name} {last_name} from {country} - {town}!')
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 4 strings - first name, last name, country and town 
* Prints information about a person in the following format: "\{firstName\} \{lastName\} from \{country\} - \{town\}!"
[/task-description]
[code-io /]
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
[code-task title="Town Info" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a function, which:

* Receives name (string), population and area (numbers)
* Prints information about a town in the following format: "Town \{name\} has population of \{population\} and area \{area\} square km."
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Berlin|Town Berlin has population of 3675000 and area 984 square km.|
|3675000||
|984||
[/slide]

[slide]
# Solution: Town Info
[code-task title="Town Info" executionStrategy="python-code" requiresInput]
[code-editor language="python"]
```
town_name = input()
population = int(input())
area = int(input())
print(f'Town {town_name} has population of {population} and area {area} square km.')
```
[/code-editor]
[task-description]
Write a function, which:

* Receives name (string), population and area (numbers)
* Prints information about a town in the following format: "Town \{name\} has population of \{population\} and area \{area\} square km."
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Berlin|Town Berlin has population of 3675000 and area 984 square km.|
|3675000||
|984||
[/slide]
