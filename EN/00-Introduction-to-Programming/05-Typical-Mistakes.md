# Typical Mistakes

[slide]
# Video

[vimeo-video videoId="342590118" startTimeInSeconds="5053" endTimeInSeconds="5538" /]

[/slide]

[slide]
# Writing Outside of the Main Method
One of the common mistakes with beginners is writing outside the body of the `Main()` **method**, because the integrated environment or the compiler can't read the given commands in the program correctly. 

Here is an example for an incorrectly written program:
```cs
static void Main(string[] args)
{
}
Console.WriteLine("Hello C#");
```

# Wrong Letter Capitalization
Another mistake is switching **capital and small letters**, and these matter for calling the commands and their correct functioning. 

Here is an example of such a mistake:
```cs
static void Main(string[] args)
{
    Console.Writeline("Hello C#");
}
```

# Missing Semicolon
The absence of **a semicolon** (`;`) in the end of the commands is one of the eternal problems of the beginner programmer. 

Skipping this sign leads to **incorrect functioning of the program** and **often the problem stays unnoticed**. 

Here is an example of a mistaken code:
```cs
static void Main(string[] args)
{
    Console.Writeline("Hello C#")
}
```

# Missing or Wrong Quotation Mark or Parenthesis
Missing **quotation mark** or **the absence of opening or closing parentheses** can also turn out to be a problem. 

Same as the semicolon, here also the problem leads to **incorrect functioning of the program** or overall to its failure. 

This mistake is hardly noticeable in a larger code. Here is an example of a program with errors:
```cs
static void Main(string[] args)
{
    Console.WriteLine("Hello C#);
}
```

This program will throw **a compile time error** and the build is going to fail, and even before that the code will become underlined, in order to point the programmer to the mistake that they'd made (the missing closing quotation mark):

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/01-typical-mistakes-csharp.png"/]

Another example is missing `{` or `}`. It may produce unexpected error messages, not always easy to understand.
```cs
class Example
{
    static void Main(string[] args)
    {
        Console.WriteLine("Hello C#);
}
```
[/slide]