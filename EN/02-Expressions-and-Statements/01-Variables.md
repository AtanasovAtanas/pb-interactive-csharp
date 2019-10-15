# Variables

[slide]
# Video

[vimeo-video videoId="341512905" startTimeInSeconds="1025" endTimeInSeconds="1719" /]

[/slide]

[slide]
# Variables
In programming, each **variable** stores a certain value of a particular type. 

For example, data types can be: number, letter, text (string), date, color, image, list and others. Here are some examples of data types:
* integer: 1, 2, 3, 4, 5, 20, …
* float: 0.5, 3.14, -1.5, …
* character (symbol): 'a', 'b', 'c', '@', 'X', …
* text (string): "Hello", "Hi", "How are you?", …
* day of week: Monday, Tuesday, …, Sunday
* date and time: 14-June-1980 6:30:00, 25-Dec-2017 23:17:22

You can also imagine that **variables** are containers for data or named areas in the memory and the data that they are storing can be read and changed at any time. 

Basically **variables** provide means for:
  * **Storing** data
  * **Retrieving** stored data
  * **Modifying** stored data
  
They are characterized by:
  * name (identifier)
  * type (of the information preserved)
  * value (stored information)

Each of the variables in C# has a name, a **type** and a **value**. 

Here is how we would declare a variable and assign it with a value at the same time:
```cs
string name = "Bob";
bool employed = true;
int age = 35;
```

If you think of the variables as boxes that hold information, this is how they would look like:

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/expressions-and-statements-boxes.png"/]

Variables can be stored in the program's:
  * Operational memory - in the execution **stack**
  * Dynamic memory - in the **heap**
[/slide]

[slide]
# Naming Conventions
In computer programming, a naming convention is a set of **rules** for choosing the name to be used for variables.

In C# the convention for naming variables is ***"camel-case"***. 

There are other naming conventions which are used in different languages such as pascal case, snake case. 

**Camel case** combines words by:
* capitalizing all words following the first word
* removing the space:
```cs
int userLoginCount;
```

**Pascal case** combines words by:
* capitalizing each word along with the first one
* removing the space:
```csharp
int UserLoginCount;
```

**Snake-case** is another naming convention, which separates words with:
* one underscore character (_)
* no spaces
* each element's initial letter usually lowercased within the compound
* the first letter either upper or lowercase:
```cs
int users_count;
string first_name;
```
[/slide]