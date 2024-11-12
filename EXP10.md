# Ex.No: 10  Pytest program for Sum of digits

### DATE: 29/10/2024                                                                          
### REGISTER NUMBER : 212222040105
### AIM: To write a python program for Fibonacci Series and generate test cases using Pytest. 

### Algorithm:

1. Write the python program for Fibonacci Series. 
2. Make sure that function name should be “def test_*():” and the line to be tested 
should have assert keyword at the beginning. 
3. Write some test cases for to be tested and save it as “test_fib.py”. 
4. Open command prompt and change the directory to where pytest and program is 
saved and type “pytest test_fib.py” and run it. 
5. Stop the program.

### Program:
```
def sumOfDigits(n):
sum = 0
while (n != 0):
sum = sum + int(n % 10)
n = int(n/10)
return sum
def test_1():
assert sumOfDigits(123) == 6
def test_2():
assert sumOfDigits(256) == 2
```


### Output:

![image](https://github.com/user-attachments/assets/4b96abc9-8ed6-4dd5-a851-0fc5eace8f1c)


### Result:
Thus, the python program for Fibonacci Series is tested using pytest and executed and output is verified successfully.


