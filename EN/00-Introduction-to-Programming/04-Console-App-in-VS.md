# Console App in Visual Studio

[slide]
# Video

[vimeo-video videoId="342590118" startTimeInSeconds="4407" endTimeInSeconds="6546" /]

[/slide]

[slide]
# Console App in Visual Studio
We already have Visual Studio and we can start it. 

Then, we create a new console project: `[File]` → `[New]` → `[Project]` → `[Visual C#]` → `[Windows]` → `[Console Application]`.

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/01.Hello-csharp-01.png"/]

We set **a meaningful name** to our program, for example `HelloCSharp`:

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/01.Hello-csharp-02.png"/]

Visual Studio is going to create for us **an empty C# program**, which we have to finish writing (VS Solution with VS Project in it, with C# source file in it, with one C# class in it, with `Main()` method in it).
[/slide]

[slide]
# Writing the Program Code
The source code of the C# program is written in the section `Main(string[] args)`, between the opening and the closing parentheses `{ }`.

This is the main method (action), that is being executed with the start of a C# program. This `Main()` method can be written in two ways:
- `static void Main(string[] args)` – with parameters from the command line (we are not going into details)
- `static void Main()` – without parameters from the command line.

Both ways are valid, as **the second one is recommended**, because it is shorter and clearer. 

By default, though, when creating a console application, Visual Studio uses the first way, which we can edit manually if we want to, and delete the part with the parameters `string[] args`.

Press `[Enter]` after **the opening parentheses** `{` and **start writing**.

The code of the program is written **inwards**, as this is a part of shaping up the text for convenience during a review and/or debugging.

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/01.Hello-csharp-03.png"/]

Write the following command:
```cs
Console.WriteLine("Hello C#");
```

Here is how our program should look like in Visual Studio:

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/01.Hello-csharp-04.png"/]

The command `Console.WriteLine("Hello C#")` in the C# language means to execute printing (`WriteLine(…)`) on the console (`Console`) and to print the text message `Hello C#`, which we should surround by quotation marks, in order to clarify that this is a text. In the end of each command in the C# language the symbol `;` is being put and it says that the command ends in that place (it doesn't continue on the next line).

This command is very typical in programming: we say a given **object** should be found (in this case the console) and some **action** should be executed upon it (in this case it is printing something that is given inside the brackets). 

More technically explained, we call the method `WriteLine(…)` from the class `Console` and give as a parameter to it a text literal `"Hello C#"`.
[/slide]

[slide]
# Starting the Program
To start the program, press `[Ctrl + F5]`. If there aren't any errors, the program will be executed. 

The result will be written on the console (in the black window):

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/01.Hello-csharp-05.png"/]

Notice that we start it with `[Ctrl+F5]`, and not only `[F5]` or with the start button in Visual Studio. 

If we use `[F5]`, the program will run shortly and right afterwards the black window will disappear, and we are not going to see the result.

Actually, the output from the program is the following text message:
```
Hello C#
```

The message **"Press any key to continue . . ."** is displayed additionally on the last line on the console after the program ends, in order to push us to see the result from the execution and to press a key to close the console.
[/slide]