# Ex.No: 4 check the given number is Armstrong number or not and inspect for failures.
### DATE: 03/09/2024                                                                         
### REGISTER NUMBER : 212222040105
### AIM: 
Write a python program to check the number is Armstrong number or not and inspect for failures.

### Algorithm:
1.  Start the program.
2.	Read an integer input number.
3.	Initialize the variables current_digit, sum = 0, and num = number.
4.	Repeat Steps 5 to 7 until num > 0
5.	current_digit = (num % 10).
6.	sum = sum + (current_digit * current_digit * current_digit). 7. Stop the program.
7.	num = num / 10.
8.	Check if sum == number. If true, print "It is an Armstrong Number." Otherwise, print "It is not an Armstrong Number."
9.	Stop the program.

### Program:
```
x = input("Enter the input: ")
if x.isnumeric():
    x = int(x)
    temp = x
    cube = 0

    while temp > 0:
        digit = temp % 10
        cube += digit ** 3
        temp //= 10

    if cube == x:
        print("Armstrong Number")
    else:
        print("Not an Armstrong Number")
else:
    print("Enter a Positive Integer.")

```
### Output:
```
1. Enter the input: 143
Not an Armstrong Number

2. Enter the input: 370
Armstrong Number

3. Enter the input: 371
Armstrong Number

4. Enter the input: 10
Not an Armstrong Number

5. Enter the input: -153
Enter a Positive Integer.

6. Enter the input: 370A
Enter a Positive Integer.

7. Enter the input: -2/3
Enter a Positive Integer.

8. Enter the input:
Enter a Positive Integer.

9. Enter the input: @123
Enter a Positive Integer.

10. Enter the input: 0
Armstrong Number
```
### Result:
Thus, the python program to check the number is Armstrong number or not implemented and the output is verified successfully.


