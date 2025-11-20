## Flowchart Workshop 2

### TABLE OF CONTENTS

<small>

- [Total & Average](#total--average)<br>
- [Multiplication Table](#multiplication-table)<br>
- [Positive Negative Zero Check](#positive-negative-zero-check)<br>
- [Interest Calculator](#interest-calculator)<br>
- [Average Temperature](#average-temperature)<br>
- [Area For Square](#area-for-square)<br>
- [Pass or Fail](#pass-or-fail)<br>
- [Factorial](#factorial)<br>
- [Calculate Discount](#calculate-discount)

</small>
<br>

### Total & Average

```pseudocode
START
    INPUT mark1,mark2,mark3
    total = mark1 + mark2 + mark3
    average = total / 3
    PRINT total
    PRINT average
END
```

<div align="center">

```mermaid
%%{init: {'flowchart': {'curve': 'linear'}} }%%
flowchart TD
    A([START]):::AZ --> B[/INPUT Marks/]:::IO
    B --> C1[Mark 1 + Mark 2 + Mark 3]:::CA
    B --> C2["(Mark 1 + Mark 2 + Mark 3)" </br> &div; Mark Amount]:::CA
    C1 --> D2[/PRINT Total/]:::IO
    C2 --> D3[/PRINT Average/]:::IO
    D2 & D3 --> E([END]):::AZ

    classDef AZ color:#fff,fill:#111111,stroke:#3,stroke-width:4px
    classDef IO color:#fff,fill:#231f2c,stroke:#3,stroke-width:3px
    classDef CA color:#fff,fill:#211832,stroke:#3,stroke-width:3px
```

</div>
</br>
    
### Multiplication Table

```pseudocode
START
    INPUT number
    FOR number FROM 1 TO 10 DO
        result = number * number
        PRINT result
    END FOR
END
```

<div align="center">

```mermaid
%%{init: {'flowchart': {'curve': 'linear'}} }%%
flowchart TD
    A([START]):::AZ --> B[/INPUT Number/]:::IO
    B --> C(For Number from 1 to 10 </br> &times; INPUT):::CA
    C --> D[/PRINT Result/]:::IO
    D --> G([END]):::AZ

    classDef AZ color:#fff,fill:#111111,stroke:#3,stroke-width:4px
    classDef IO color:#fff,fill:#231f2c,stroke:#3,stroke-width:3px
    classDef CA color:#fff,fill:#211832,stroke:#3,stroke-width:3px
```

</div>
</br>

### Positive Negative Zero Check

```pseudocode
START
    INPUT number
    IF number > 0 THEN
        PRINT "Positive"
    ELSE IF number < 0 THEN
        PRINT "Negative"
    ELSE
        PRINT "Zero"
    END IF
END
```

<div align="center">

```mermaid
%%{init: {'flowchart': {'curve': 'linear'}} }%%
flowchart TD
    A([START]):::AZ --> B[/INPUT Number/]:::IO
    B --> C{Number > 0}:::DE
    C -- Yes ---> D[/PRINT Positive/]:::IO
    C -- No --> E{Number < 0}:::DE
    E -- Yes ---> F[/PRINT Negative/]:::IO
    E -- No --> G[/PRINT Zero/]:::IO
    D & F & G --> H([END]):::AZ

    classDef AZ color:#fff,fill:#111111,stroke:#3,stroke-width:4px
    classDef IO color:#fff,fill:#231f2c,stroke:#3,stroke-width:3px
    classDef DE color:#fff,fill:#2a1f36,stroke:#3,stroke-width:3px
```

</div>
</br>

### Interest Calculator

```pseudocode
START
    INPUT amount,rate,years
    interest = (amount * rate) * years
    PRINT interest
END
```

<div align="center">

```mermaid
%%{init: {'flowchart': {'curve': 'linear'}} }%%
flowchart TD
    A([START]):::AZ --> B[/INPUT</br>Amount, Rate & Years/]:::IO
    B --> C("(Amount &times; Rate)" &times; Years):::CA
    C --> D[/PRINT Interest/]:::IO
    D --> E([END]):::AZ

    classDef AZ color:#fff,fill:#111111,stroke:#3,stroke-width:4px
    classDef IO color:#fff,fill:#231f2c,stroke:#3,stroke-width:3px
    classDef CA color:#fff,fill:#211832,stroke:#3,stroke-width:3px
```

</div>
</br>

### Average Temperature

```pseudocode
START
    INITIALIZE daycounter TO 1
    INITIALIZE totaltemp TO 0

    WHILE daycounter <= 7 DO
        INPUT temperature
        totaltemp = totaltemp + temperature
        daycounter = daycounter + 1
    END WHILE

    averagetemp = totaltemp / 7
    PRINT averagetemp
END
```

<div align="center">

```mermaid
%%{init: {'flowchart': {'curve': 'linear'}} }%%
flowchart TD
    A([START]):::start --> B[INITIALIZE<br/>Day Counter = 1]:::process
    A --> C[INITIALIZE<br/>Total Temp = 0]:::process
    B & C --> D{Day Counter < 7}:::decision
    D -- YES --> E[/INPUT<br/>Temperature/]:::input
    E --> F[Total Temp =<br/>Total Temp + Temperature]:::calc
    F --> G[Day Counter =<br/>Day Counter + 1]:::calc
    G --> D
    D -- NO --> H[Average Temp =<br/>Total Temp &div; 7]:::calc
    H --> I[/PRINT<br/>Average Temperature/]:::output
    I --> J([END]):::start

    classDef start color:#fff,fill:#111111,stroke:#3,stroke-width:4px
    classDef process color:#fff,fill:#211832,stroke:#3,stroke-width:4px
    classDef decision color:#fff,fill:#2a1f36,stroke:#3,stroke-width:4px
    classDef calc color:#fff,fill:#211832,stroke:#3,stroke-width:4px
    classDef input color:#fff,fill:#231f2c,stroke:#3,stroke-width:4px
    classDef output color:#fff,fill:#231f2c,stroke:#3,stroke-width:4px
```

</div>
</br>

### Area For Square

```pseudocode
START
    INPUT side1, side2
    area = side1 * side2
    PRINT area
END
```

<div align="center">

```mermaid
%%{init: {'flowchart': {'curve': 'linear'}} }%%
flowchart TD
    A([START]):::AZ --> B[/INPUT Length & Width/]:::IO
    B --> C(Length &times; Width):::CA
    C --> D[/PRINT Area/]:::IO
    D --> E([END]):::AZ

    classDef AZ color:#fff,fill:#111111,stroke:#3,stroke-width:4px
    classDef IO color:#fff,fill:#231f2c,stroke:#3,stroke-width:3px
    classDef CA color:#fff,fill:#211832,stroke:#3,stroke-width:3px
```

</div>
</br>

### Pass or Fail

```pseudocode
START
    INPUT averagemarks
    IF averagemarks >= 50 THEN
        PRINT "Pass"
    ELSE
        PRINT "Fail"
    END IF
END
```

<div align="center">

```mermaid
%%{init: {'flowchart': {'curve': 'linear'}} }%%
flowchart TD
    A([START]):::AZ --> B[/INPUT Average Marks/]:::IO
    B --> C{If Average Marks &ge; 50}:::DE
    C -- Yes ---> D[/PRINT Pass/]:::IO
    C -- No --> E[/PRINT Fail/]:::IO
    D & E --> F([END]):::AZ

    classDef AZ color:#fff,fill:#111111,stroke:#3,stroke-width:4px
    classDef IO color:#fff,fill:#231f2c,stroke:#3,stroke-width:3px
    classDef DE color:#fff,fill:#2a1f36,stroke:#3,stroke-width:3px
```

</div>
</br>

### Calculate Factorial

```pseudocode
START
    INPUT number
    IF number >= 0 THEN
        INITIALIZE factorial TO 1
        FOR x FROM 1 TO number DO
            factorial = factorial * x
        END FOR
        PRINT factorial
    ELSE
        PRINT "Invalid input"
    END IF
END
```

<div align="center">

```mermaid
%%{init: {'flowchart': {'curve': 'linear'}} }%%
flowchart TD
    A([START]):::AZ --> B[/INPUT Number/]:::IO
    B --> C{If Number &ge; 0}:::DE
    C -- Yes ---> D[Initialize Factorial = 1]:::CA
    D --> E[For x from 1 to Number </br> Factorial = Factorial &times; x]:::CA
    E --> G[/PRINT Factorial/]:::IO
    C -- No --> H[/PRINT Invalid input/]:::IO
    G & H --> I([END]):::AZ

    classDef AZ color:#fff,fill:#111111,stroke:#3,stroke-width:4px
    classDef IO color:#fff,fill:#231f2c,stroke:#3,stroke-width:3px
    classDef DE color:#fff,fill:#2a1f36,stroke:#3,stroke-width:3px
    classDef CA color:#fff,fill:#211832,stroke:#3,stroke-width:3px
```

</div>
</br>

### Calculate Discount

```pseudocode
START
    INPUT price
    IF price > 1000 THEN
        discount = price * 0.1
        price = price - discount
    END IF
    PRINT price
END
```

<div align="center">

```mermaid
%%{init: {'flowchart': {'curve': 'linear'}} }%%
flowchart TD
    A([START]):::AZ --> B[/INPUT Price/]:::IO
    B --> C{If Price &gt; 1000}:::DE
    C -- Yes ---> D[Discount = Price &times; 0.1]:::CA
    D --> E[Price = Price - Discount]:::CA
    E --> F[/PRINT Price/]:::IO
    C -- No --> F
    F --> G([END]):::AZ

    classDef AZ color:#fff,fill:#111111,stroke:#3,stroke-width:4px
    classDef IO color:#fff,fill:#231f2c,stroke:#3,stroke-width:3px
    classDef DE color:#fff,fill:#2a1f36,stroke:#3,stroke-width:3px
    classDef CA color:#fff,fill:#211832,stroke:#3,stroke-width:3px
```

</div>
