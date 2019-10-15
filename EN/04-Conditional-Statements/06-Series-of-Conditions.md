# Sequence of If-Else Conditions

[slide]
# Video

[vimeo-video videoId="341532970" startTimeInSeconds="4534" endTimeInSeconds="5115" /]

[/slide]

[slide]
# Sequence of If-Else Conditions
Sometimes we need to do a sequence of conditions before we decide what actions our program will execute. 

In such cases, we can apply the construction `if-else if ... -else` **in series**.

For this purpose, we use the following format:
```cs
if (condition)
{
  // condition body;
}
else if (second condition)
{
  // condition body;
}
else if (third condition)
{
  // condition body;
}
…
else
{
  // else construction body;
}
```
[/slide]

[slide]
# Example: Digits in English
Print the digits in the range of 1 to 9 (digits are read from the console) in English. 

We can read the digit and then, through a **sequence of conditions** we print the relevant English word:
```cs live
int num = int.Parse(Console.ReadLine());

if (num == 1)
{
    Console.WriteLine("one");
}
else if (num == 2)
{
    Console.WriteLine("two");
}
else if (num == 3) 
{
    Console.WriteLine("three");
} 
else if (num == 4) 
{
    Console.WriteLine("four");
}
else if (num == 5) 
{
    Console.WriteLine("five");
}
else if (num == 6) 
{
    Console.WriteLine("six");
}
else if (num == 7) 
{
    Console.WriteLine("seven");
}
else if (num == 8) 
{
    Console.WriteLine("eight");
}
else if (num == 9)
{
    Console.WriteLine("nine");
} 
else 
{
    Console.WriteLine("number too big");
}
```

The program logic from the above example **sequentially compares** the input number from the console with the digits from 1 to 9, when **each following comparison is being performed only in case the previous comparison is not true**. 

Eventually, if none of the `if` statements are true, the last `else` **clause** is performed.
[/slide]