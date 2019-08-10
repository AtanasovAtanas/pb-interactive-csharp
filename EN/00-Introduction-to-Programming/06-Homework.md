[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Print "Hello C#"
[html]
<style>
@import url('https://fonts.googleapis.com/css?family=Lato&display=swap');

#swal2-content {
  font-family: 'Lato', sans-serif;
}

.fab fa-facebook {
  color: #3e4c5d;
  background: transparent;
}

.fb-xfbml-parse-ignore {
  padding: 10px;
  color: #3e4c5d;
  font-family: 'Lato', sans-serif;
}
</style>
<script async defer crossorigin="anonymous"
  src="https://connect.facebook.net/en_GB/sdk.js#xfbml=1&version=v4.0&appId=430304805003&autoLogAppEvents=1"></script>

  <script src="https://cdn.jsdelivr.net/npm/sweetalert2@8"></script>
  <script src="https://kit.fontawesome.com/d01480363c.js"></script>
  <script>
let constantMock = window.fetch;
let taskFinished = false;
window.fetch = function () {
  if (taskFinished) {
    return new Promise((resolve, reject) => {
      constantMock.apply(this, arguments)
        .then(res => {
          resolve(res);
        })
        .catch((err) => {
          reject(err);
        });
    })
  }

  return new Promise((resolve, reject) => {
    constantMock.apply(this, arguments)
      .then(async (response) => {
        let data = await response.clone().json();
        let taskResult = data.executionResult.taskResult;
        if (taskResult) {
          let isRightAnswer = taskResult.testResults[0].resultType === 'CorrectAnswer';

          if (isRightAnswer) {
            Swal.fire({
              title: 'Good Job!',
              text: 'Got 100/100 on the first task!',
              footer: '<div id="fb-root"></div><i class="fab fa-facebook"></i><div class="fb-share-button" data-href="https://softuni.org" data-layout="button_count" data-size="small"><a target="_blank" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fsoftuni.org%2F&amp;src=sdkpreparse" class="fb-xfbml-parse-ignore">Share to Facebook</a></div>'
            });

            taskFinished = true;
          }
          // } else {
          //   Swal.fire({
          //     type: 'error',
          //     title: 'Oops...',
          //     text: '0/100'
          //   })
          // }
        }

        resolve(response);
      })
      .catch((error) => {
        // Swal.fire({
        //   type: 'error',
        //   title: 'Oops...',
        //   text: 'Something went wrong!'
        // })
        reject(error);
      })
  });
}
  </script>
[/html]
[code-task title="Print Hello C#" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a C# program, which:

Prints "Hello C#" on the console
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
Hello C#
[/output]
[/test]
[/tests]
[/code-task]
[html]
    <style>
    table.iotable{
    border:2px solid white;
    padding: 5px;
    width: 100%;
    border-radius: 4px;
    border-spacing: 10px;
    font-size: 20px;
}
table th{
    text-decoration: underline;
    text-align: center;
    padding-bottom: 3px;
    padding: 1.0%;
}
table tbody td{
    text-align: center;
    border-bottom:1px solid white;
    padding: 1.0%;
}

table tbody tr:nth-child(even){
    background-color: #234465;
    color: white
}

table tr:last-child{
  border: none;
}

table tbody tr:nth-child(odd){
    color: white;
    border-bottom: 1px solid gray;
}

table tr td:not(:last-child):hover{
    text-decoration: underline;
}
    }
  </style>
<table class="iotable">
    <thead>
      <tr>
        <th>#</th>
        <th>Input</th>
        <th>Output</th>
        <th>Comment</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>1</td>
        <td>22222222</td>
        <td>22222222</td>
        <td>22222222</td>
      </tr>
      <tr>
        <td>2</td>
        <td>3333333333</td>
        <td>3333333333</td>
        <td>3333333333</td>
      </tr>
      <tr>
        <td>3</td>
        <td>444444444444</td>
        <td>444444444444</td>
        <td>444444444444</td>
      </tr>
      <tr>
        <td>4</td>
        <td>444444444444</td>
        <td>444444444444</td>
        <td>444444444444</td>
      </tr>
      <tr>
        <td>5</td>
        <td>444444444444</td>
        <td>444444444444</td>
        <td>444444444444</td>
      </tr>
    </tbody>
  </table>
[/html]
[/slide]

[slide]
# Solution: Print "Hello C#"
[code-task title="Print Hello C#" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine("Hello C#");
  }
}
```
[/code-editor]
[task-description]
Write a C# program, which:

Prints "Hello C#" on the console
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
Hello C#
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Problem: Calculate and Print 5 * 5
[code-task title="Calculate and Print 5 * 5" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a C# program, which:

* Calculates the value of 5 * 5
* Prints the result
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
25
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Calculate and Print 5 * 5
[code-task title="Calculate and Print 5 * 5" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine(5 * 5);
  }
}
```
[/code-editor]
[task-description]
Write a C# program, which:

* Calculates the value of 5 * 5
* Prints the result
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
25
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Problem: Name and Expression
[code-task title="Name and Expression" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program to print 'Catlyn' at the first line and calculate and print the expression 5 + 3 at the second line
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
Catlyn
8
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Name and Expression
[code-task title="Name and Expression" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine("Catlyn");
    Console.WriteLine(5 + 3);
  }
}
```
[/code-editor]
[task-description]
Write a program to print 'Catlyn' at the first line and calculate and print the expression 5 + 3 at the second line
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
Catlyn
8
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Problem: Calculations
[code-task title="Calculations" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which calculates and prints the value of the following expressions:

* 5 + 3 \* 2
* 4 \* (2 + 3)
* (2 + 5)  \*  (8 - 2) \/ 7
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
11
20
6
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Calculations
[code-task title="Calculations" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
class Program
{
  static void Main()
  {
    Console.WriteLine(5 + 3 * 2);
    Console.WriteLine(4 * (2 + 3));
    Console.WriteLine(
      (2 + 5) * (8 - 2) / 7);
  }
}
```
[/code-editor]
[task-description]
Write a program, which calculates and prints the value of the following expressions:

* 5 + 3 \* 2
* 4 \* (2 + 3)
* (2 + 5)  \*  (8 - 2) \/ 7
[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
11
20
6
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Problem: Square of 7 * 7 Stars
[code-task title="Square of 7 * 7 Stars" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

Prints a square of 7 * 7 stars like this:

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Square of 7 * 7 Stars
[code-task title="Square of 7 * 7 Stars" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
    {
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
      Console.WriteLine("* * * * * * *");
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

Prints a square of 7 * 7 stars like this:

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

\* \* \* \* \* \* \*

[/task-description]
[code-io /]
[tests]
[test]
[input]
[/input]
[output]
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
\* \* \* \* \* \* \*
[/output]
[/test]
[/tests]
[/code-task]
[/slide]
