# Basic Calculator Application Test Cases

The repository contains test cases for a basic calculator application. The cases cover a wide range of scenarios including basic arithmetic, order of operations, edge cases, large numbers, decimal handling, invalid inputs, chained calculations.


## **1. Arithmetic Tests**

These tests cover basic arithmetic operations like addition, subtraction, multiplication, division and some special cases for whole and decimal numbers.


## **1.1. Addition, Substraction, Multiplication, Division - whole numbers**

| **Number 1** | **Number 2** | **Operation** | **Expected Result**          | **Explanation**                                                       |
|--------------|--------------|---------------|------------------------------|-----------------------------------------------------------------------|
| 6            | 4            | +             | 10                           | Add two positive whole numbers.                                       |
|-6            |-4            | +             | -10                          | Add two negative whole numbers.                                       |
| 7            | -4           | +             | 3                            | Add one positive and one negative whole number.                       |
| 0            | 7            | +             | 7                            | Add zero to a whole number.                                           |
| 7            | 0            | +             | 7                            | Add a whole number to zero.                                           |
| -6           | 4            | +             | -2                           | Add a negative and a positive whole number.                           |
| 7            | 4            | -             | 3                            | Subtract two positive whole numbers.                                  |
| -7           | 4            | -             | -11                          | Subtract a positive whole number from a negative.                     |
| 0            | 7            | -             | -7                           | Subtract a positive whole number from zero.                           |
| 6            | 0            | -             | 6                            | Subtract zero from a positive number.                                 |
| -7           | -4           | -             | -3                           | Subtract a negative number from a negative.                           |
| 6            | 4            | ×             | 24                           | Multiply two positive whole numbers.                                  |
| -6           | -4           | ×             | 24                           | Multiply two negative whole numbers.                                  |
| 7            | 0            | ×             | 0                            | Multiply a whole number by zero.                                      |
| -7           | 0            | ×             | 0                            | Multiply a negative number by zero.                                   |
| 12           | 6            | ÷             | 2                            | Divide two positive whole numbers.                                    |
| 12           | 0            | ÷             | Error ("Cannot divide by 0") | Divide a positive whole number by 0 - Division by zero is not allowed.|
| 0            | 6            | ÷             | 0                            | Divide zero by a positive whole number.                               |
| 6            | -6           | ÷             | -1                           | Divide a positive by a negative whole number.                         |
| -12          | -6           | ÷             | 2                            | Divide a negative by a negative whole number.                         |
| 0            | 0            | ÷             | Error ("Cannot divide by 0") | Divide 0 by 0 - Division by zero is not allowed.                      |



## **1.2. Addition, Substraction, Multiplication, Division - decimals**

| **Number 1** | **Number 2** | **Operation** | **Expected Result**          | **Explanation**                                                  |
|--------------|--------------|---------------|------------------------------|------------------------------------------------------------------|
| 2.4          | 4.1          | +             | 6.5                          | Add two positive decimal numbers.                                |
| -3.4         | -2.2         | +             | -5.6                         | Add two negative decimal numbers.                                |
| 6.8          | -2.9         | +             | 3.9                          | Add a positive decimal and a negative decimal.                   |
| 7.6          | 4.2          | -             | 3.4                          | Subtract two positive decimals.                                  |
| -6.4         | 4.7          | -             | -11.1                        | Subtract a positive decimal from a negative.                     |
| 6.3          | 4.2          | ×             | 26.46                        | Multiply two positive decimal numbers.                           |
| -6.4         | -4.1         | ×             | 26.24                        | Multiply two negative decimal numbers.                           |
| 7.0          | 0            | ×             | 0                            | Multiply a decimal by zero.                                      |
| 7.2          | 3.6          | ÷             | 2                            | Divide two positive decimals.                                    |
| 14.0         | 0            | ÷             | Error ("Cannot divide by 0") | Divide a positive decimal by 0 - Division by zero is not allowed.|
| 0            | 6.4          | ÷             | 0                            | Divide zero by a positive decimal.                               |
| 7.5          | 0.75         | ÷             | 10                           | Divide a positive decimal by a smaller decimal.                  |
| -8.4         | 0            | ÷             | Error ("Cannot divide by 0") | Divide a negative decimal by 0 - Division by zero is not allowed.|
| 4.9          | -3.6         | ÷             | -1.36                        | Divide a positive decimal by a negative decimal.                 | 



## **1.3. Addition, Substraction, Multiplication, Division - whole numbers and decimals**

| **Number 1** | **Number 2** | **Operation** | **Expected Result** | **Explanation**                                           |
|--------------|--------------|---------------|---------------------|-----------------------------------------------------------|
| 6            | 2.5          | +             | 8.5                 | Add a a whole number to decimal.                          |
| -4           | 3.8          | +             | -0.2                | Add a negative whole number to a positive decimal.        |
| 7.1          | -3           | +             | 4.1                 | Add a decimal to a negative whole number.                 |
| 0            | 4.5          | +             | 4.5                 | Add zero to a decimal.                                    |
| -2.3         | 6            | +             | 3.7                 | Add a negative decimal to a positive whole number.        |
| 8            | 3.5          | -             | 4.5                 | Subtract a decimal from a whole number.                   |
| -6.2         | 4            | -             | -10.2               | Subtract a positive whole number from a negative decimal. |
| 5.7          | -2           | -             | 7.7                 | Subtract a negative whole number from a decimal.          |
| 0            | 3.9          | -             | -3.9                | Subtract a decimal from zero.                             |
| 4            | 2.5          | ×             | 10                  | Multiply a whole number by a decimal.                     |
| -3           | 2.7          | ×             | -8.1                | Multiply a negative whole number by a positive decimal.   |
| 5.2          | -2           | ×             | -10.4               | Multiply a positive decimal by a negative whole number.   |
| 0            | 4.5          | ×             | 0                   | Multiply zero by a decimal.                               |
| -2.5         | 3            | ×             | -7.5                | Multiply a negative decimal by a positive whole number.   |
| 8            | 2.0          | ÷             | 4                   | Divide a whole number by a decimal.                       |
| -9           | 3.0          | ÷             | -3                  | Divide a negative whole number by a positive decimal.     |
| 0            | 3.2          | ÷             | 0                   | Divide zero by a decimal.                                 |



## **2. Order of Operation Tests**

These tests verify that the calculator respects the correct order of operations - parentheses, multiplication/division, addition/subtraction.

| **Operation**    | **Expected Result** | **Explanation**                                                                                 |
|------------------|---------------------|-------------------------------------------------------------------------------------------------|
| 3 + 5 * 2        | 13                  | Multiplication first: 5 * 2 = 10, then addition: 3 + 10 = 13.                                   |
| (2 + 3) * 2      | 10                  | Parentheses first: (2 + 3) = 5, then multiplication: 5 * 2 = 10.                                |
| 4 + 6 / 2        | 7                   | Division first: 6 / 2 = 3, then addition: 4 + 3 = 7.                                            |
| 8 - (2 + 2)      | 4                   | Parentheses first: (2 + 2) = 4, then subtraction: 8 - 4 = 4.                                    |
| 10 / 2 * 4       | 20                  | Left-to-right execution: (10 / 2) * 4 = 20.                                                     |
| 3.5 + 5.2 * 2    | 13.9                | Multiplication first: 5.2 * 2 = 10.4, then addition 3.5 + 10.4 = 13.9.                          |
| (2.3 + 3.7) * 2  | 12.0                | Parentheses first: (2.3 + 3.7) = 6.0, then multiplication 6.0 * 2 = 12.0.                       |
| 10 - 4 / 2 + 1   | 9                   | Division first: 4 / 2 = 2, then subtraction: 10 - 2 = 8, then addition: 8 + 1 = 9.              |
| 5 * (2 + 3) - 4  | 21                  | Parentheses first: (2 + 3) = 5, then multiplication: 5 * 5 = 25, then subtraction: 25 - 4 = 21. |



## **3. Large Numbers Tests**

These tests ensure that the calculator can handle large numbers without issues.

| **Number 1**     | **Number 2**     | **Operation** | **Expected Result**      | **Explanation**                         |
|------------------|------------------|---------------|--------------------------|-----------------------------------------|
| 1000000          | 2000             | *             | 2000000000               | Large number multiplication.            |
| 9999999999999    | 1                | +             | 10000000000000           | Addition of large numbers.              |
| 9876543210       | 1234567890       | /             | 8.000000001              | Large number division.                  |
| 123456789012345  | 123456789012345  | -             | 0                        | Subtraction of large identical numbers. |
| 1000000000000    | 999999999999     | *             | 999999999999000000000000 | Large multiplication result.            |



## **4. Chained Calculations Tests**

These tests demonstrate how chained calculations work for both whole numbers and decimal numbers.
The order of operations follows **PEMDAS**, but in chained calculations, the result of one step is used directly in the next.

| **Steps**             | **Expected Result** | **Explanation**                                                  |
|-----------------------|---------------------|------------------------------------------------------------------|
| 2 + 3 = × 4           | 20                  | First add (2 + 3 = 5), then multiply (5 × 4 = 20).               |
| 10 ÷ 2 = + 5          | 10                  | First divide (10 ÷ 2 = 5), then add (5 + 5 = 10).                |
| 8 ÷ 4 = × 3           | 6                   | First divide (8 ÷ 4 = 2), then multiply (2 × 3 = 6).             |
| 6 + 2 = ÷ 4           | 2                   | First add (6 + 2 = 8), then divide (8 ÷ 4 = 2).                  |
| 2.5 + 3.5 = × 4.0     | 24.0                | First add (2.5 + 3.5 = 6.0), then multiply (6.0 × 4.0 = 24.0).   |
| 10.5 ÷ 2.5 = + 5.0    | 9.2                 | First divide (10.5 ÷ 2.5 = 4.2), then add (4.2 + 5.0 = 9.2).     |
| 8.4 + 2.6 = ÷ 5.0     | 2.2                 | First add (8.4 + 2.6 = 11.0), then divide (11.0 ÷ 5.0 = 2.2).    |



## **5. Invalid Inputs Tests**

These tests demonstrate how the calculator should handle invalid inputs.

| **Input**             | **Expected Result**            | **Explanation**                                                               |
|-----------------------|--------------------------------|-------------------------------------------------------------------------------|
| a                     | Error ("Invalid Input")        | Letters are not allowed.                                                      |
| 1 +                   | Waiting for input              | Mathematical operations cannot be performed if one of the numbers is missing. |
| 5 * ()                | Error ("Invalid Syntax")       | Empty parentheses or missing operands result in invalid syntax.               |
| 3 + + 4               | Error ("Invalid Syntax")       | Repeated or misplaced operators cause a syntax error.                         |
| 6 ÷ 0                 | Error ("Cannot Divide by Zero")| Division by zero is not allowed.                                              |


## **6. Edge Test Cases**

| **Input**                                 | **Expected Result**            | **Explanation**                                                                     |
|-------------------------------------------|--------------------------------|-------------------------------------------------------------------------------------|
| 9999999999999999999999999 + 1             | Error ("Overflow")             | Numbers that exceed the calculator's maximum value may trigger overflow errors.     |
| 9999999999999999 / 9999999999999999       | 1                              | Division of extremely large numbers might stress test precision and rounding errors.|
| 0.0000000001 + 0.0000000001               | 0.0000000002                   | Testing precision with very small decimal numbers.                                  |
| 1 / 3                                     | 0.3333333333333333...          | Long division and testing precision with recurring decimals.                        |
