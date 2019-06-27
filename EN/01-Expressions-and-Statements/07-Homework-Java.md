[slide]
# Homework - Java
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Calculate Speed
[code-task title="Calculate Speed" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
    // Write code here
  }
}
```
[/code-editor]
[task-description]

Write a program to calculate the speed by time and distance:
  * Read 2 floating-point numbers: distance and time
  * Calculate the speed needed to travel a given distance for given time
  * Print the calculated result

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|15|7.5| 
|2|| 
[/slide]

[slide]
# Solution: Calculate Speed
[code-task title="Calculate Speed" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      double distance = Double.parseDouble(scanner.nextLine());
      double time = Double.parseDouble(scanner.nextLine());
      double speed = distance / time;
      System.out.println(speed);
    }
}
```
[/code-editor]
[task-description]

Write a program to calculate the speed by time and distance:
  * Read 2 floating-point numbers: distance and time
  * Calculate the speed needed to travel a given distance for given time
  * Print the calculated result

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|15|7.5| 
|2|| 
[/slide]

[slide]
# Problem: Currency Converter
[code-task title="Currency Converter" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program to convert from USD to EUR:
  * Read a **floating-point number**: the **dollars** to be converted 
  * Convert dollars to euro (use fixed rate of dollars to euro: **0.88**)
  * Print the converted value in **euro**

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|17|14.96| 
|87|76.56|
[/slide]

[slide]
# Solution: Currency Converter
[code-task title="Currency Converter" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      double dollars = Double.parseDouble(scanner.nextLine());
      double euros = dollars * 0.88; 
      System.out.println(euros);
    }
}
```
[/code-editor]
[task-description]

Write a program to convert from USD to EUR:
  * Read a **floating-point number**: the **dollars** to be converted 
  * Convert dollars to euro (use fixed rate of dollars to euro: **0.88**)
  * Print the converted value in **euro**

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|17|14.96| 
|87|76.56|
[/slide]

[slide]
# Problem: Area of Triangle
[code-task title="Area of Triangle" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program to calculate a triangle area:

  * Read from input a side **a** and height for that side **ha**
  * Calculate the area of a triangle by the side and height
  * Print the **area**, formatted to the **2nd digit** after decimal point

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5|25.00 | 
|10| | 
[/slide]

[slide]
# Solution: Area of Triangle
[code-task title="Area of Triangle" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      double a = Double.parseDouble(scanner.nextLine());
      double h = Double.parseDouble(scanner.nextLine());
      double area = (a * h) / 2;
      System.out.printf("%.2f", area);
    }
}
```
[/code-editor]
[task-description]

Write a program to calculate a triangle area:

  * Read from input a side **a** and height for that side **ha**
  * Calculate the area of a triangle by the side and height
  * Print the **area**, formatted to the **2nd digit** after decimal point

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5|25.00| 
|10|| 
[/slide]

[slide]
# Problem: Four Operations
[code-task title="Four Operations" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
  * **Reads** 2 real numbers from the **console**
  * Performs **4 arithmetic operations** on the obtained 2 numbers, in the following order: **+, -, *, /**
  * **Formats** and **prints** the results like this example:

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5|5.00 + 10.00 = 15.00| 
|10|5.00 - 10.00 = -5.00|
||5.00 * 10.00 = 50.00|
||5.00 / 10.00 = 0.50|
[/slide]

[slide]
# Solution: Four Operations
[code-task title="Four Operations" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      double num1 = Double.parseDouble(scanner.nextLine());
      double num2 = Double.parseDouble(scanner.nextLine());
      System.out.printf("%.2f + %.2f = %.2f%n", num1, num2, num1 + num2);
      System.out.printf("%.2f - %.2f = %.2f%n", num1, num2, num1 - num2);
      System.out.printf("%.2f * %.2f = %.2f%n", num1, num2, num1 * num2);
      System.out.printf("%.2f / %.2f = %.2f%n", num1, num2, num1 / num2);
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
  * **Reads** 2 real numbers from the **console**
  * Performs **4 arithmetic operations** on the obtained 2 numbers, in the following order: **+, -, *, /**
  * **Formats** and **prints** the results like this example:

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5|5.00 + 10.00 = 15.00| 
|10|5.00 - 10.00 = -5.00|
||5.00 * 10.00 = 50.00|
||5.00 / 10.00 = 0.50|
[/slide]

[slide]
# Problem: Days to Minutes
[code-task title="Days to Minutes" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program to convert from days to minutes:
  * Read a single **integer** (the **days** to be converted)
  * Convert the days to minutes (use calculations)
  * Print the **minutes**

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|2|2880|
|5|7200|
[/slide]

[slide]
# Solution: Days to Minutes
[code-task title="Days to Minutes" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      int days = Integer.parseInt(scanner.nextLine());
      int hours = days * 24;
      int minutes = hours * 60;
      System.out.println(minutes);
    }
}
```
[/code-editor]
[task-description]

Write a program to convert from days to minutes:
  * Read a single **integer** (the **days** to be converted)
  * Convert the days to minutes (use calculations)
  * Print the **minutes**

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|2|2880|
|5|7200|
[/slide]

[slide]
# Problem: Circle Area and Perimeter
[code-task title="Circle Area and Perimeter" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;
 
public class Program {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program to calculate a circle area and perimeter:
  * Read a floating-point number: the radius of a circle
  * Calculate the area and perimeter of a circle
  * Print the calculated values

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|7|Area = 153.938040|
||Perimeter = 43.982297|

[/slide]

[slide]
# Solution: Circle Area and Perimeter
[code-task title="Circle Area and Perimeter" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      double radius = Double.parseDouble(scanner.nextLine());
      double area = radius * radius * Math.PI;
      double perimeter = 2 * Math.PI * radius;
      System.out.printf("Area = %f%n", area);
      System.out.printf("Perimeter = %f%n", perimeter);
    }
}
```
[/code-editor]
[task-description]

Write a program to calculate a circle area and perimeter:
  * Read a floating-point number: the radius of a circle
  * Calculate the area and perimeter of a circle
  * Print the calculated values

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|7|Area = 153.938040|
||Perimeter = 43.982297|
[/slide]

[slide]
# Problem: Person Info
[code-task title="Person Info" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner; 

public class Program {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
  * Reads 4 lines of **strings**: first name, last name, country and town 
  * Prints information about a person in the following format: "**{firstName} {lastName} from {country} - {town}!**"

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Kelly|Kelly Smith from Ireland - Cork!|
|Smith||
|Ireland||
|Cork||
[/slide]

[slide]
# Solution: Person Info
[code-task title="Person Info" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      String firstName = scanner.nextLine();
      String lastName = scanner.nextLine();
      String country = scanner.nextLine();
      String town = scanner.nextLine();
      System.out.printf("%s %s from %s - %s!",   firstName, lastName, country, town);
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
  * Reads 4 lines of **strings**: first name, last name, country and town 
  * Prints information about a person in the following format: "**{firstName} {lastName} from {country} - {town}!**"

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Kelly|Kelly Smith from Ireland - Cork!|
|Smith||
|Ireland||
|Cork||
[/slide]

[slide]
# Problem: Town Info
[code-task title="Town Info" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
  * Reads **3 lines** of input: **name** (string), **population** and **area** (integers)
  * Prints information about a town in the following format: "**Town {name} has population of {population} and area {area} square km.**"

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Berlin|Town Berlin has population of 3675000 and area 984 square km.|
|3675000||
|984||
[/slide]

[slide]
# Solution: Town Info
[code-task title="Town Info" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      String townName = scanner.nextLine();
      int population = Integer.parseInt(scanner.nextLine());
      int area = Integer.parseInt(scanner.nextLine()); 
      System.out.printf("Town %s has population of %d and area %d  square km.", townName, population, area);
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
  * Reads **3 lines** of input: **name** (string), **population** and **area** (integers)
  * Prints information about a town in the following format: "**Town {name} has population of {population} and area {area} square km.**"

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Berlin|Town Berlin has population of 3675000 and area 984 square km.|
|3675000||
|984||
[/slide]
