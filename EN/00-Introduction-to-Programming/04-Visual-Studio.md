[slide]
# Installing Visual Studio
We begin with the installation of the integrated environment **Microsoft Visual Studio** (Community, version 2017, latest as of June 2017). 

Installing later versions of Visual Studio (like Visual Studio 2019 and Visual Studio 2021) should be very similar.

The **Community** version of Visual Studio (VS) is distributed freely by Microsoft and can be downloaded from: https://www.visualstudio.com/vs/community. The installation is typical for Windows with `[Next]`, `[Next]` and `[Finish]`, but it's important to include the components for **"desktop development"** and **"ASP.NET"**. 

It is not necessary to change the rest of the settings for the installation.

The next lines describe in detail the steps for the installation of Visual Studio (version Community 2017). 

After we download the installation file and start it, the following screen appears:
[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.visual-studio-1.png"/]

Press the `[Continue]` button and you will see the screen bellow:
[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.visual-studio-2.png"/]

A screen with the installation panel of Visual Studio is being loaded.
[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.visual-studio-3.png"/]

Put a check mark on `[Universal Windows Platform development]`, `[.NET desktop development]` and `[ASP.NET and web development]`, then press the `[Install]` button. Basically, this is everything.

Installation of Visual Studio begins, and a screen like the one bellow will appear:
[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.visual-studio-5.png"/]

After Visual Studio is installed, an informative screen will appear. Press the `[Launch]` button to start it.
[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.visual-studio-6.png"/]

Upon **starting VS** a screen appears like the one bellow. 

On it you can choose whether you will enter Visual Studio using a Microsoft account. 

For now, we choose to continue without being logged into our Microsoft account, and therefore we choose the option `[Not now, maybe later.]`. 
[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.visual-studio-7.png"/]

The next step is to choose **the color theme**, in which Visual Studio is visualized. The choice here lays completely on the preferences of the user and it doesn't matter which option will be chosen.
[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.visual-studio-8.png"/]

Press the `[Start Visual Studio]` button and the main view of Visual Studio Community will be displayed:
[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/00.visual-studio-9.png"/]

That's all. You are ready to work with Visual Studio.
[/slide]

[slide]
# Project Solutions and Projects in Visual Studio
Before we start working with Visual Studio, it is necessary to get familiar with the concepts of a **Visual Studio Solution** and a **Visual Studio Project**, which are an inevitable part of it.

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/august/assets/VS-solutions-and-projects.png"/]

**Visual Studio Project** represents "the **project**" we are working on. In the beginning, these will be our console applications, which we are going to learn writing with the help of the current book, the resources in it and the course Programming Basics in SoftUni. 

With deeper learning, time and practice, these projects will move into the direction of desktop applications, web applications and other developments. 

A project in VS **logically groups multiple files** constructing a given application or a component. 

A **C# project** contains one or more **C# source files**, configuration files and other resources. In every C# source file, there is one or more definition of types (classes or other definitions). 

In the classes there are methods (actions), and they contain a sequence of commands. It sounds complicated, but with bigger projects a structure like this one is very convenient and allows good organization of the work files.

**Visual Studio Solution** represents a container (a work **solution**), in which **a few projects are logically bound**. 

The purpose of the binding of these VS Projects is to create an opportunity for the code from any of the projects to collaborate with the code from the rest of the VS projects, to ensure the application or the website to work correctly. 

When the software product or service that we develop is big, it is built as a **VS Solution**, and this Solution is split into projects (VS Projects) and inside each project there are folders with source files.

This hierarchical organization is much more convenient with more serious projects (let's say over 50 000 lines of code).

For **smaller projects** VS Solutions and VS Projects are **complicating the work**, rather than helping, but you will get used to it quickly.
[/slide]

[slide]
# Video

[vimeo-video videoId="342590118" startTimeInSeconds="4041" endTimeInSeconds="4405" /]

[/slide]