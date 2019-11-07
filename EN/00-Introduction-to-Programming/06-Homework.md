[slide]
# Homework
Welcome to the homework. 

Now we are going to write a couple of console applications, by which we are going to make a few more steps into programming. 

We have prepared some problems for you to solve.

Let's solve a few problems to confirm what we have learned.

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/homeowrk.png"/]

[html]
let table = document.createElement('table');
table.innerHTML = `<tr>
<th>Problem Name</th>
<th>Results</th>
<th>Fail/Pass</th>
</tr>
</thead>
<tbody>
</tbody>`;

table.style.border = "1px solid white";
table.style.margin = "0";
table.style.padding = "0";
table.style.borderSpacing = "12px 4px";

let problems = Array.from(Array.from(document.querySelectorAll('.collapsible-lesson-navigation-section')).filter((el) => el.textContent.includes('Homework') && el.textContent.includes('Problem:'))[0].querySelector('section.lesson-navigation-section').querySelectorAll('a.content-link')).map((el, i) => { return {el, i} }).filter((a) =>
a.el.querySelector('h4').textContent.includes('Problem:')).reduce((acc, curr, i) => {
acc.push({problemName: curr.el.textContent, href: curr.el.href, index: curr.i});
return acc;
},[]);

const homeworkElement = Array.from(document.querySelectorAll('a.content-link')).filter((a) => a.children[0].textContent === 'Homework')[0];

homeworkElement.addEventListener('click', () => {

let spanResults = document.querySelectorAll('span.tests-top-result-text');

console.log(spanResults);

let homeArticle = Array.from(document.querySelectorAll('article')).filter((article) => article.querySelector('h4.slide-title').textContent === 'Homework').slice(-1)[0];

problems.forEach((problem) => {

let tr = document.createElement('tr');

let tdName = document.createElement('td');
tdName.textContent = problem.problemName.split(':')[1];

let tdResult = document.createElement('td');
let result = spanResults[problem.index - 1].textContent.split('/')[0];
tdResult.textContent = result;

let tdPassOrFail = document.createElement('td');
tdPassOrFail.textContent =  (+result) < 100 ? 'Failed' : 'Pased';

tr.appendChild(tdName);
tr.appendChild(tdResult);
tr.appendChild(tdPassOrFail);

table.querySelector('tbody').appendChild(tr)
})

homeArticle.appendChild(table);
});
[/html]

[/slide]

[slide]
# Problem: Print "Hello C#"
[code-task title="Print Hello C#" taskId="p-01" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
[/slide]

[slide]
# Problem: Calculate and Print 5 * 5
[code-task title="Calculate and Print 5 * 5" taskId="p-02" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
# Problem: Name and Expression
[code-task title="Name and Expression" taskId="p-03" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
Write a program to print 'Catlyn' on the first line and calculate and print the result of the expression 5 + 3 on the second line
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
[code-task title="Calculations" taskId="p-04" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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
# Problem: Square of 7 * 7 Stars
[code-task title="Square of 7 * 7 Stars" taskId="p-05" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code"]
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

```
* * * * * * *
* * * * * * *
* * * * * * *
* * * * * * *
* * * * * * *
* * * * * * *
* * * * * * *
```

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
# My Results

[/slide]

[slide]
# Video

[vimeo-video videoId="342590118" startTimeInSeconds="5539" endTimeInSeconds="6548" /]

[/slide]