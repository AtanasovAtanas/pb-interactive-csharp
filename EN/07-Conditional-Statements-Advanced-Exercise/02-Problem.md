[slide]
# Problem: Fruit or Vegetable
[code-task title="Fruit or Vegetable" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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
# Description

Your task is to write a program that takes as input from the user **name of a product** and checks if the product is **fruit** or **vegetable**.

- The fruits "**fruit**" are **banana**, **apple**, **kiwi**, **cherry**, **lemon** and **grapes**
- The vegetables "**vegetable**" are **tomato**, **cucumber**, **pepper** and **carrot**
- Everything else is "**unknown**"

# Output

Print on the console "**fruit**", "**vegetable**" or "**unknown**" according to the product name.

# Example

| **Input** | | **Output** |      
| --- | --- | --- |                 
| banana | | fruit |                   

| **Input** | | **Output** |      
| --- | --- | --- |                   
| tomato | | vegetable | 

| **Input** | | **Output** |      
| --- | --- | --- |                  
| water | | unknown |

\* **Hint**: use conditional **if** statement with logical "**or**" - operator "\|\|".
[/task-description]
[tests]
[test]
[input]
banana
[/input]
[output]
fruit
[/output]
[/test]
[test]
[input]
apple
[/input]
[output]
fruit
[/output]
[/test]
[test]
[input]
kiwi
[/input]
[output]
fruit
[/output]
[/test]
[test]
[input]
cherry
[/input]
[output]
fruit
[/output]
[/test]
[test]
[input]
lemon
[/input]
[output]
fruit
[/output]
[/test]
[test]
[input]
grapes
[/input]
[output]
fruit
[/output]
[/test]
[test]
[input]
tomato
[/input]
[output]
vegetable
[/output]
[/test]
[test]
[input]
cucumber
[/input]
[output]
vegetable
[/output]
[/test]
[test]
[input]
pepper
[/input]
[output]
vegetable
[/output]
[/test]
[test]
[input]
carrot
[/input]
[output]
vegetable
[/output]
[/test]
[test]
[input]
water
[/input]
[output]
unknown
[/output]
[/test]
[test]
[input]
beer
[/input]
[output]
unknown
[/output]
[/test]
[/tests]
[code-io /]
[/code-task] 
[/slide]