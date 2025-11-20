# 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and determine whether it is even or odd.

## Pseudocode
```
START
    INPUT number
    IF (number % 2 == 0) THEN
        PRINT The number is EVEN
    ELSE
        PRINT The number is ODD
    ENDIF
END
```

## Flowchart
```mermaid
flowchart TD
    A([START]) --> B[/INPUT number/]
    B --> C{number % 2 == 0 ?}
    C --> |Yes| D[/PRINT The number is EVEN/]
    C --> |No| E[/PRINT The number is ODD/]
    D --> F([END])
    E --> F([END])
```


# 2. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs marks for 3 subjects, calculates the total and average, and displays both.

## Pseudocode
```
START
    INPUT A,B and C
    total = 0, average = 0
    total = A + B + C
    average = total / 3
    PRINT "Total marks is "+total
    PRINT "Average is "+average
END
````

## Flowchart
```mermaid
flowchart
    A([START]) --> B[/Input numbers A, B and C/]
    B --> C[total = 0, average = 0]
    C --> D[total = A+B+C]
    D --> E[average = total/3]
    E --> F[/PRINT total/]
    F --> G[/PRINT average/]
    G --> H([END])
```

# 3. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its multiplication table from 1 to 10 using a loop.

## Pseudocode
```
START
    INPUT number
    FOR i = 1 to 10 DO
        PRINT (i+"*"+number+"="+(i*number))
    END FOR
END
```

## Flowchart
```mermaid
flowchart TD
    A([START]) --> B[/input number/]
    B --> C[i = 1]
    C --> D{i <= 10 ?}
    D --> |Yes| E[/PRINT i times number equals i times number/]
    E --> F[i = i+1]
    F --> D
    D --> |No| F([END])
```

# 4. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether it is positive, negative, or zero.

## Pseudocode
```
START
    INPUT number
    IF number > 0 THEN
        PRINT "The number is Positive"
    ELSE IF number < 0 THEN
        PRINT "The number is Negative"
    ELSE
        PRINT "The number is Zero"
    END IF
END
````

## Flowchart
```mermaid
flowchart TD
    A([START]) --> B[/INPUT number/]
    B --> C{number > 0 ?}
    C --> |Yes| D[/PRINT Number is Positive/]
    C --> |No| E{number < 0 ?}
    E --> |Yes| F[/PRINT Number is Negative/]
    E --> |No| G[/PRINT Number is Zero/]
    D --> H([END])
    F --> H([END])
    G --> H([END])
```

# 5. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple interest using the formula

## Pseudocode
```
START
    INPUT P, R and T
    SI = 0.0
    SI = (P * R * T) / 100
    PRINT "The Simple Interest is "+SI
END
```

## Flowchart
```mermaid
flowchart TD
    A([START]) --> B[/INPUT P, R and T/]
    B --> C[SI = 0.0]
    C --> D[SI equals multiply P,R and T and divide the result by 100]
    D --> E[/PRINT SI/]
    E --> F([END])
```

# 6. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the temperature of 7 days, finds the average temperature, and displays it.

## Pseudocode
```
START
    total = 0, average = 0
    REPEAT 7 TIMES
        INPUT temp
        total = total + temp
    ENDREPEAT
    average = total / 7
    PRINT "Average Temperature is ", average
END
````

## Flowchart
```mermaid
flowchart TD
    A([START]) --> B[total = 0, average = 0, count = 1]
    B --> C{count <= 7 ?}
    C --> |Yes| D[/INPUT Temp/]
    D --> E[total = total + Temp]
    E --> F[count = count + 1]
    F --> C
    C --> |No| G[average = total / 7]
    G --> H[/PRINT average/]
    H --> I([END])
```

# 7. Calculate Area of a Rectangle

Create an algorithm and flowchart to input length and width, calculate the area (Area = Length × Width), and display the result.

## Pseudocode
```
START
    INPUT L and W
    Area = 0
    Area = L * W
    PRINT "Area of Rectangular is "+Area
END
````

## Flowchart
```mermaid
flowchart TD
    A([START]) --> B[/INPUT L and W/]
    B --> C[Area = 0]
    C --> D[Area equals multiplication of L and W]
    D --> E[/PRINT Area/]
    E --> F([END])
```

# 8. Determine Pass or Fail

Write the algorithm and draw the flowchart for a program that takes a student's average marks and displays "Pass" if average ≥ 50, otherwise "Fail".

## Pseudocode
```
START
    INPUT marks A, B, C, D and E
    total = 0, average = 0
    total = A+B+C+D+E
    average = total / 5
    IF average >= 50 THEN
        PRINT Pass
    ELSE
        PRINT Fail
    END IF
END
````

## Flowchart
```mermaid
flowchart TD
    A([START]) --> B[/INPUT Marks A, B, C, D and E/]
    B --> C[total = 0, average = 0]
    C --> D[total = add all five marks]
    D --> E[average equals total divided by 5]
    E --> F{average >= 50 ?}
    F --> |Yes| G[/PRINT Pass/]
    F --> |No| H[/PRINT Fail/]
    G --> I([END])
    H --> I([END])
```

# 9. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and calculate its factorial using a loop.

## Pseudocode
```
START
    INPUT num
    fact = 1
    FOR i = 1 TO num DO
        fact = fact * i 
    END FOR
    PRINT "Factorial of a Number is +fact"
END
````

## Flowchart
```mermaid
flowchart TD
    A([START]) --> B[/INPUT num/]
    B --> C[fact = 1]
    C --> D[i = 1]
    D --> E{i <= num}
    E --> |Yes| F[fact equals fact multiplies i]
    F --> G[i = i+1]
    G --> E
    E --> |No| H[/PRINT fact/]
    H --> I([END])
```


# 10. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the purchase amount and gives a 10% discount if the amount is greater than 1000.

## Pseudocode
```
START
    INPUT amt
    discountedAmt = 0.0
    IF (amt > 1000) THEN
        discountedAmt = (amt * 90) / 100
        PRINT "Amount to be paid after the discound is "+discountedAmt
    ELSE
        PRINT "Amount to be paid is "+amt
    END IF
END
````

## Flowchart
```mermaid
flowchart TD
    A([START]) --> B[/INPUT amt/]
    B --> C[discountedAmt = 0.0]
    C --> D{amt > 1000 ?}
    D --> |Yes| E[discountedAmt equals multiplication of amt and 90, then divide the total by 100]
    E --> F[/PRINT discountedAmt/]
    D --> |No| G[/PRINT amt/]
    F --> H([END])
    G --> H([END])
```