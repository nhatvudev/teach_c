## **Basic data types in C/C++**
- Integer:
    + `char` (1 byte)
    + `unsigned char` (1 byte)
    + `short` (2 bytes)
    + `unsigned short` (2 bytes)
    + `int` (its size depends on the target platform).
    + `unsigned int` (its size depends on the target platform)
    + `long` or `long int` (8 bytes)
    + `long long` or `long long int` (8 bytes)
- Floating-point
    + `float` (4 bytes)
    + `double` (8 bytes)
- Boolean (only on C++):
    + `true`
    + `false`

**Remarks:** 
```
- In C, there isn't built-in boolean type, so a non-zero integer is equivalent to true, and a zero integer is equivalent to false.
- There is a header which define "true" as 1 and "false" as 0: "stdbool.h"
```

## **variable Declaration & initialization**
```C
data_type var_name; // declaration
data_type var_name = value; // declaration & initialization at same line.
```

## **Basic statement types in C/C++**
- Declaration, Definition, Initialization
- Expression
- Code Block `{...}` (can contain more than 1 statement)
- Condition: if/else, switch/case
- Loop: for, while, do/while
- break, continue, goto
- Null (`;`)
- Exception handling statements (only for C++)

## **if/else**
- Type 1:
```C
if (condition) statement;

if (condition)
    statement;
```

- Type 2:
```C
if (condition) statement; else statement;

if (condition)
    statement;
else
    statement;
```

- Type 3:
```C
if (condition) statement; else if (condition) statement; ... else statement;

if (condition)
    statement;
else if (condition)
    statement;
...
else
    statements;
```

- Remarks:
    + condition is a truth value: non-zero (true) / zero (false)

## **switch/case**

```C
switch (value):
{
    case value1a:
    case value1b:
    ...
        statements;
    
    case value2a:
    case value2b:
    ...
        statements;

    ...
    default:
        statements;
}
```

## **for loop**
```C
for (init_statement; condition; loop_expression) statement;

for (init_statement; condition; loop_expression)
    statement;
```

## **while loop**
```C
while (condition) statement;

while (condition)
    statement;
```

## **do/while loop**
```C
do { } while (condition);

do {

} while (condition);

do
{

} while (condition);
```

## **Function**

## **Array**

## **C-type String**

## **struct**

## **union**

## **enum**

## **Pointer to data**

## **Dynamic allocation**

## **Pointer to function**

## **File handling**