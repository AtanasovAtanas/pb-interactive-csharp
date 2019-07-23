[slide]

# How does Computing Work?
Computers are machines that process data. The process of receiving 
information is called **input**. The input needs to be stored in
the computer memory and it can be done by using variables. 

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/expressions-and-statements-3.png"/]

[/slide]

[slide]
# Variables
In programming, each **variable** stores a certain value of a particular type. 
For example, data types can be: number, letter, text (string), date, color, 
image, list and others. Here are some examples of data types:

* integer: 1, 2, 3, 4, 5, 20, …
* float: 0.5, 3.14, -1.5, …
* character (symbol): 'a', 'b', 'c', '@', 'X', …
* text (string): "Hello", "Hi", "How are you?", …
* day of week: Monday, Tuesday, …, Sunday
* date and time: 14-June-1980 6:30:00, 25-Dec-2017 23:17:22

You can also imagine that **variables** are containers for data or named areas in the memory
and the data that they are storing can be read and changed at any time. Basically **variables**
provide means for:
  * **Storing** data
  * **Retrieving** stored data
  * **Modifying** stored data
  
They are characterized by:
  * name (identifier)
  * type (of the information preserved)
  * value (stored information)

Each of the variables in C# has a name, a type and a value. Here is how we would 
declare a variable and assign it with a value at the same time:
```csharp
int age = 25;
```

Variables can be stored in the program's:
  * Operational memory - in the execution stack
  * Dynamic memory - in the heap
[/slide]
