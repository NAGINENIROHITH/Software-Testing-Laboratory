# Ex.No: 3 To check the number is prime or not and inspect for failures.
 
### DATE: 24/09/2024                                                                          
### REGISTER NUMBER : 212222040105
### AIM: 
Write a python program to check the number is prime or not and inspect for failures.
 
### Algorithm:
1. Start the program.
2. Get the number to be checked from the user.
3. If the number is less than or equal to 1, return "Not Prime".
4. If the number is 2, return "Prime".
5. Start the iteration from 3, For each iteration:
6. If the number is divisible by the current iteration value, return "Not Prime".
7. If the number is not divisible by any value from 2 to the square root, return "Prime".
8. Stop the program.

### Program:
```
num = input("Enter a number: ")
flag = 0

if num.isnumeric(): 
    z = int(num)
    if z == 2:  # 2 is a prime number
        flag = 1
    elif z > 2:
        flag = 1  
        for i in range(2, z // 2 + 1):  
            if z % i == 0:
                flag = 0  
                break
    if flag == 1:
        print("Prime Number")
    else:
        print("Not a Prime Number")
else:
    print("Enter a Positive Number")

```

### Output:
```
1. Enter a number: 2
Prime Number

2. Enter a number: 10
Not a Prime Number

3.  Enter a number: -3
Enter a Positive Number

4.   Enter a number: 3
Prime Number

5.  Enter a number: 
Enter a Positive Number

6. Enter a number: 22/7
Enter a Positive Number

7. Enter a number: 3.14
Enter a Positive Number

8. Enter a number: 3A
Enter a Positive Number

9. Enter a number: 11A
Enter a Positive Number

10. Enter a number: 11
Prime Number
```

### Result:
Thus, the python program to check the number is prime or not is implemented and the output is verified successfully.