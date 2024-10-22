## Ex.No: 2 Matrix Multiplication
## DATE: 03/09/2024
## REGISTER NUMBER : 212222040105
## AIM:
Write a python program for matrix multiplication and inspect for failures.

## Algorithm:
Start the program.
Create empty list formatrix1, matrix2 and result.
Get the rows and columns count from the user.
Get the values of two matrix.
Perform matrix multiplication and store the answer in result.
Stop the program.
## Program:
```
r1, c1 = input("Enter row and column count in matrix 1: ").split()
r2, c2 = input("Enter row and column count in matrix 2: ").split()

matrix1 = []
matrix2 = []
result = []

if r1.isnumeric() and c1.isnumeric() and r2.isnumeric() and c2.isnumeric():
    r1 = int(r1)
    r2 = int(r2)
    c1 = int(c1)
    c2 = int(c2)

    if c1 != r2:
        print("Matrix multiplication not possible")
    elif max(r1, c1, r2, c2) > 20 or min(r1, c1, r2, c2) == 0:
        print("Matrix multiplication not possible")
    else:
        print("Enter elements for matrix 1:")
        for i in range(r1):
            a = []
            for j in range(c1):
                a.append(int(input("<- ")))
            matrix1.append(a)

        print("Enter elements for matrix 2:")
        for i in range(r2):
            a = []
            for j in range(c2):
                a.append(int(input("<- ")))
            matrix2.append(a)

        for i in range(r1):
            result.append([0] * c2)

        for i in range(r1):
            for j in range(c2):
                for k in range(c1):
                    result[i][j] += matrix1[i][k] * matrix2[k][j]

        print("Resulting matrix:")
        for i in range(r1):
            for j in range(c2):
                print(result[i][j], end=" ")
            print()
else:
    print("Enter a valid number")
```
## Output:
```
FAILURE CASES:
1. Enter the size of a: 2 3
Enter the size of b: 2 3
Matrix multiplication is not possible.
Reason to fail: to do multiplication of matrices the number of columns in matrix ―a[] should be
equal to the number of rows in matrix in b[]

2. Enter the size of a: p q
Enter the size of b: q s
Matrix multiplication is not possible.
Reason to fail: to do multiplication of matrices the number of columns in matrix ―a[]
should be equal to number of rows in matrix ―bl, and rows & columns should be integer
values.

3. Enter the size of a: 1.5 2
Enter the size of b: 2 3
Matrix multiplication is not possible.
Reason to fail: to do multiplication of matrices the number of columns in matrix ―al should be
equal to number of rows in matrix ―bl, and rows & columns should be integer

4. Enter the size of a: 350
480 Enter the size of b:
480 620
Matrix multiplication is not possible.
Reason to fail: size of buffer will be not be sufficient to handle this multiplication.

5. Enter the size of a: -
1 -2 Enter the size of
b: -2 3
Matrix multiplication is not possible.
Reason to fail: to do multiplication of matrices the number of columns in matrix ―al should
be equal to number of rows in matrix ―bl, and rows & columns should be positive integer values.
```
## Result:
Thus, the python program for matrix multiplication is implemented and the causes for its failure is introspected successfully.
