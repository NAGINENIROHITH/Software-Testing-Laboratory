# Ex.No: 1 Write programs in Python Language to demonstrate the working of followingconstructs with possible test cases: a) do…while b) while…do c) if …else d) switch e) for 

### DATE: 27/08/2024                                                                      
### REGISTER NUMBER :  212222040105

### AIM:  
To write python programs for do…while, while, for, switch and if…else and test with possible test 
Cases 

### Algorithm:
1. Start the program.
2. Create separate files for each given program.
3. Write simple program for each construct.
4.  the program with possible test cases.
5. Stop the program.
### Program:
## do...while:
```
def display(): 
    start=input("Enter a positive value for START: ") 
    end=input("Enter a positive value for END: ") 
    if start.isnumeric() and end.isnumeric(): 
        while True: 
            start=int(start) 
            end=int(end) 
            print(start,end=" ") 
            if start<end: 
                start+=1 
            else: 
                break 
    else: 
        print("Enter a valid positive number.") 
display() 
```
## OUTPUT:
```
Enter a positive value for START: 1
Enter a positive value for END: 4
1 2 3 4

Enter a positive value for START: -10 
Enter a positive value for END: 5 
Enter a valid positive number.

Enter a positive value for START: hello 
Enter a positive value for END: y
Enter a valid positive number.

Enter a positive value for START:
Enter a positive value for END:
Enter a valid positive number.
```
## while...do:
```
start=input("Enter a positive value for START: ") 
end=input("Enter a positive value for END: ") 
if start.isnumeric() and end.isnumeric(): 
    start=int(start) 
    end=int(end) 
    while start<end: 
        print(start) 
        start+=1 
else: 
    print("Enter a valid positive number.")
```
## Output:
```
Enter a positive value for START: 1 
Enter a positive value for END: 4
1 2 3 4

Enter a positive value for START: -10 
Enter a positive value for END: 5 
Enter a valid positive number.

Enter a positive value for START: abc 
Enter a positive value for END: 100 
Enter a valid positive number.

Enter a positive value for START: 
Enter a positive value for END: 
Enter a valid positive number.
```
## switch:
```
def switch(): 
    switcher={ 0:"even", 1:"odd" } 
    n=input('Enter a value for N: ') 
    try: 
        n=int(n) 
        print(switcher[n%2]) 
    except ValueError: 
        print("Enter a valid number.") 

switch() 
```
## Output:
```
Enter a value for N: 1 
odd

Enter a value for N: -10 
even

Enter a value for N: hello 
Enter a valid number.

Enter a value for N:
Enter a valid number.
```
## if..else:
```
def compare(): 
    a=input("Enter a value for A: ") 
    b=input("Enter a value for B: ") 
    try: 
        a=int(a) 
        b=int(b) 
        if a>b: 
            print("A is greater than B") 
        elif a<b: 
            print("B is greater than A") 
        else: 
            print("A is equal to B") 
    except ValueError: 
        print("Enter a valid number.")

compare()

```
## Output:
```
Enter a value for A: 1 
Enter a value for B: 1 
A is equal to B.

Enter a value for A: -10 
Enter a value for B: 5 
B is greater than A.

Enter a value for A: hello 
Enter a value for B: y 
Enter a valid number.

Enter a value for A:
Enter a value for B:
Enter a valid number.
```
## for:
```
def iterate(): 
    string=input("Enter a string: ") 
    for i in string: 
        print(ord(i),end=" ") 
iterate()

```
## Output:
```
Enter a string: say 
115 97 121

Enter a string: 1543 
49 53 52 51

Enter a string:

```


### Result:
Thus, the python program to demonstrate the working of given constructs is implemented and the output is verified successfully.


