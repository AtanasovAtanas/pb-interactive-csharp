# Infinite Loops

[slide]
# Video

[vimeo-video videoId="341948488" startTimeInSeconds="4530" endTimeInSeconds="5061" /]

[/slide]

[slide]
# Infinite Loops
So far, we were introduced to `for` loop, learning what structure it has and how it is applied. 

Now, we need to understand what an **infinite loop** is and when it occurs.

We call an **infinite loop** one that **repeats infinitely** the performance of its body. 

Infinite `for` occurs when there is **no condition to end the loop**.

Here is what a `for` loop with no end condition looks like:
```cs live
for ( ; ; ) 
{
  Console.WriteLine("Hello World");
}
```

Usually, it results from a programming error - for example, where the conditions for exit are incorrectly written. 

An infinite loop is not dangerous. It can, however, be annoying when it occurs.

So you have to be careful not to cause one by accident.
[/slide]