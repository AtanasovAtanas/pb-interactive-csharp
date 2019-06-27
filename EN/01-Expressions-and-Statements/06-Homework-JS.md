[slide]
# Homework - JS
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Calculate Speed
[code-task title="Calculate Speed" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function calculateSpeed (input) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 2 parameters - distance and time
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
[code-task title="Calculate Speed" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function calculateSpeed (input) {
  let distance = Number(input.shift());
  let time = Number(input.shift());
  let speed = distance / time;
  console.log(speed);
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives 2 parameters - distance and time
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
# Problem: Currency Converter
[code-task title="Currency Converter" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function currencyConverter (input) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single parameter - the dollars to be converted 
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
[code-task title="Currency Converter" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function currencyConverter (input) {
  let dollars = Number(input.shift());
  let euros = dollars * 0.88; 
  console.log(euros);
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single parameter - the dollars to be converted 
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
# Problem: Inches to Centimeters
[code-task title="Inches to Centimeters" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function inchesToCentimeters (input) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single - the inches to be converted
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
[code-task title="Inches to Centimeters" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function inchesToCentimeters (input) {
  let inches = Number(input.shift());
  let centimeters = inches * 2.54;
  console.log(centimeters);
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single parameter - the inches to be converted
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
# Problem: Four Operations
[code-task title="Four Operations" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function fourOperations(input){
    // Write code here
}
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
[code-task title="Four Operations" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function fourOperations (input) {
  let num1 = Number(input.shift());
  let num2 = Number(input.shift());
  console.log(`${num1} + ${num2} = ${num1 + num2}`);
  console.log(`${num1} - ${num2} = ${num1 - num2}`);
  console.log(`${num1} * ${num2} = ${num1 * num2}`);
  console.log(`${num1} / ${num2} = ${num1 / num2}`);
}
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
[code-task title="Days to Minutes" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function daysToMinutes (input) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single parameter (days)
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
[code-task title="Days to Minutes" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function daysToMinutes (input) {
  let days = Number(input.shift());
  let hours = days * 24;
  let minutes = hours * 60;
  console.log(minutes);
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single parameter (days)
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
# Problem: Circle Area and Perimeter
[code-task title="Circle Area and Perimeter" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function circleArea (input) {
   // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single parameter - the radius of a circle
* Calculates the area and perimeter of a circle
* Prints the calculated values formatted to the 2nd decimal
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output
|       Input       | Output |
|-------------------|--------|
|7|Area = 153.94|
||Perimeter = 43.98|
[/slide]

[slide]
# Solution: Circle Area and Perimeter
[code-task title="Circle Area and Perimeter" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function circleArea (input) {
  let radius = Number(input.shift());
  let area = radius * radius * Math.PI;
  let perimeter = 2 * Math.PI * radius;
  console.log(`Area = ${area.toFixed(2)}`);
  console.log(`Perimeter = ${perimeter.toFixed(2)}`);
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives a single number - the radius of a circle
* Calculates the area and perimeter of a circle
* Prints the calculated values formatted to the 2nd decimal
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output
|       Input       | Output |
|-------------------|--------|
|7|Area = 153.94|
||Perimeter = 43.98|
[/slide]

[slide]
# Problem: Person Info
[code-task title="Person Info" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function personInfo (input) {
   // Write your code here
}
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
[code-task title="Person Info" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function personInfo (input) {
  let firstName = input.shift();
  let lastName = input.shift();
  let country = input.shift();
  let town = input.shift();
  console.log(`${firstName} ${lastName} from ${country} - ${town}!`);
}
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
[code-task title="Town Info" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function townInfo (input) {
  // Write your code here
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives name, population and area
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
[code-task title="Town Info" executionStrategy="javascript-code" requiresInput]
[code-editor language="javascript"]
```
function townInfo (input) {
  let townName = input.shift();
  let population = Number(input.shift());
  let area = Number(input.shift());
  console.log(`Town ${townName} has population of ${population} and area ${area} square km.`);
}
```
[/code-editor]
[task-description]
Write a function, which:

* Receives name, population and area
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