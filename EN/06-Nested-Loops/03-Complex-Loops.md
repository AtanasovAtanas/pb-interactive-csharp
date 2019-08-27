[slide]
# Loop with a Step
**The step** is that **part** of the `for` loop construction that tells **how** much to **increase** or **decrease** the value of its **leading** variable. 

It is declared the last in the skeleton of the `for` loop.

Most often, we have **a size of 1**, and in this case, instead of writing `i += 1` or `i -= 1`, we can use the `i++` or `i--` operators. 

If we want our step to be **different than 1**, when increasing, we use the `i +=` + `step size` operator, and when decreasing, the `i -=` + `step size`. 

With step of 10, the loop would look like this:
```csharp
for (int i = 1; i <= 100; i += 10)
{
    Console.WriteLine(i);
}
```
[/slide]

[slide]
# Problem: Numbers from N to 1
[code-task title="Numbers form N to 1" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads an integer number **n**
* Prints the numbers from **n** to **1** 
[/task-description]
[tests]
[test]
[input]
5
[/input]
[output]
5
4
3
2
1
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|100|100|
||99|
||98|
||...|
||1|
[/slide]

[slide]
# Solution: Numbers from N to 1
[code-task title="Numbers form N to 1" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      for (int i = n; i >= 1; i--) 
      {
          Console.WriteLine(i);
      }
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads an integer number **n**
* Prints the numbers from **n** to **1** 
[/task-description]
[tests]
[test]
[input]
5
[/input]
[output]
5
4
3
2
1
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|100|100|
||99|
||98|
||...|
||1|
[/slide]

[slide]
# Problem: Numbers from 1 to N with Step 3
[code-task title="Numbers from 1 to N with Step 3" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads an integer number **n**
* Prints the numbers from **1** to **n** with step **3**
[/task-description]
[tests]
[test]
[input]
10
[/input]
[output]
1
4
7
10
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|7|1|
||4|
||7|
[/slide]

[slide]
# Solution: Numbers from 1 to N with Step 3
[code-task title="Numbers from 1 to N with Step 3" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      for (int i = 1; i <= n; i += 3) 
      {
          Console.WriteLine(i);
      }
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads an integer number **n**
* Prints the numbers from **1** to **n** with step **3**
[/task-description]
[tests]
[test]
[input]
10
[/input]
[output]
1
4
7
10
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|7|1|
||4|
||7|
[/slide]

[slide]
# Problem: Even Powers of 2
[code-task title="Even Powers of 2" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

* Reads a number **n**
* Prints the even powers of 2 to 2^**n**: 2^0, 2^2, 2^4, 2^8, …, 2^n
[/task-description]
[tests]
[test]
[input]
3
[/input]
[output]
1
4
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|1|
||4|
||16|
||...|
||1024|
[/slide]

[slide]
# Solution: Even Powers of 2
[code-task title="Even Powers of 2" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
  public static void Main()
  {
      int n = int.Parse(Console.ReadLine());
      int num = 1;
      for (int i = 0; i <= n; i += 2)
      {
          Console.WriteLine(num);
          num = num * 2 * 2;
      }
  }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number **n**
* Prints the even powers of 2 to 2**n**: 20, 22, 24, 28, …, 2n
[/task-description]
[tests]
[test]
[input]
3
[/input]
[output]
1
4
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|1|
||4|
||16|
||...|
||1024|
[/slide]

[slide]
# Video

[vimeo-video videoId="342526930" startTimeInSeconds="1773" endTimeInSeconds="3216" /]

[/slide]