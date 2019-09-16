[slide]
# Problem: Travelling
[code-task title="Travelling" executionType="tests-execution" executionStrategy="csharp-dot-net-core-code" requiresInput]
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

Annie likes to travel and she wants this year to visit **several** different destinations. When she choose a destination, she will decide how **much money she\'ll need** to go there and she will **start saving money**. When she saved **enough**, she will be able to travel.

# Input / Output

- From the **console** every time will be **read first destination and the minimum budget** which will be needed for the trip.
- It will then be read a **few sums** that Annie saves while working and **when she succeed in saving enough** for the trip, **she will go**, **as you should print on the console the following message**:

    "Going to \{destination\}!"

- When Annie visit all the destinations she wants, **instead of destination she will enter** "End" and the program will end.

# Example

| **Input** | | **Output** |
| --- | --- | --- | 
| Greece | | Going to Greece! |
| 1000 | | Going to Spain! |
| 200 | | |
| 200 | | |
| 300 | | |
| 100 | | |
| 150 | | |
| 240 | | |
| Spain | | |
| 1200 | | |
| 300 | | |
| 500 | | |
| 193 | | |
| 423 | | |
| End | | |
[/task-description]
[tests]
[test]
[input]
Greece
1000
200
200
300
100
150
240
Spain
1200
300
500
193
423
End
[/input]
[output]
Going to Greece!
Going to Spain!
[/output]
[/test]
[test]
[input]
France
2000
300
300
200
400
190
258
360
Portugal
1450
400
400
200
300
300
Egypt
1900
1000
280
300
500
End
[/input]
[output]
Going to France!
Going to Portugal!
Going to Egypt!
[/output]
[/test]
[test]
[input]
Maldives
2500
1000
340
50
50
50
50
700
700
End
[/input]
[output]
Going to Maldives!
[/output]
[/test]
[test]
[input]
Bulgaria
500
200
100
300
Austria
700
200
200
200
200
End
[/input]
[output]
Going to Bulgaria!
Going to Austria!
[/output]
[/test]
[test]
[input]
Africa
3000
1000
5000
America
2000
2500
China
4000
2000
1800
1800
End
[/input]
[output]
Going to Africa!
Going to America!
Going to China!
[/output]
[/test]
[test]
[input]
Estonia
1000
300
200
200
300
Peru
3000
2000
1000
Uganda
1000
1000
UAE
5000
3000
4000
Germany
2000
2000
Portugal
2050
3000
Portugal
2050
3000
Portugal
2050
3000
Portugal
2050
3000
Portugal
2050
3000
End
[/input]
[output]
Going to Estonia!
Going to Peru!
Going to Uganda!
Going to UAE!
Going to Germany!
Going to Portugal!
Going to Portugal!
Going to Portugal!
Going to Portugal!
Going to Portugal!
[/output]
[/test]
[test]
[input]
End
[/input]
[output]
[/output]
[/test]
[test]
[input]
France
3000
50
50
50
50
50
50
50
50
50
50
50
250
100
106
280
400
400
50
400
600
End
[/input]
[output]
Going to France!
[/output]
[/test]
[test]
[input]
Russia
15000
4500
300
300
3000
2000
4500
5000
Japan
1500.600
67.60
26.4052345
250.78
450.78945
578.76
98.60
260.84
End
[/input]
[output]
Going to Russia!
Going to Japan!
[/output]
[/test]
[test]
[input]
South Africa
2000
1000
1000
Egypt
300
150
100
20
20
20
End
[/input]
[output]
Going to South Africa!
Going to Egypt!
[/output]
[/test]
[test]
[input]
Zambia
3700.250
450.300
450.20414
600.43
640.23
824.50
1200.46
End
[/input]
[output]
Going to Zambia!
[/output]
[/test]
[test]
[input]
Albania
350.23414
45.24
23.124
123.144
145.23556
45.2345
End
[/input]
[output]
Going to Albania!
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]