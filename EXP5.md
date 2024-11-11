# Ex.No:5 BINARY SEARCH (check whether the Binary Search and inspect for failures).
# REGISTER NUMBER : 212222040105
### DATE: 10/09/2024
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
def binary_search(arr, x): 
    low = 0
    high = len(arr) - 1

    while low <= high: 
        mid = (high + low) // 2
        
        # Check if x is at mid
        if arr[mid] < x:
            low = mid + 1
        elif arr[mid] > x:
            high = mid - 1  
        else:
            return mid  
    
    return -1  

arr = [2, 3, 4, 10, 40]
x = input("Enter the element to be searched: ")

try:
    x = int(x)  # Convert input to integer
    result = binary_search(arr, x)
    
    if result != -1:
        print("Element is present at index", str(result))
    else:
        print("Element is not present in the array")
except:
    print("Enter a valid input!")
```
### Output:
```
1. Enter the element to be searched: 10
Element is present at index 3

2. Enter the element to be searched: A
Enter a valid input!

3. Enter the element to be searched: 40
Element is present at index 4

4. Enter the element to be searched: 2
Element is present at index 0

5. Enter the element to be searched: -3
Element is not present in the array

6. Enter the element to be searched: 3
Element is present at index 1

7. Enter the element to be searched: 4A
Enter a valid input!

8. Enter the element to be searched: 
Enter a valid input!

9. Enter the element to be searched: 4
Element is present at index 2

10. Enter the element to be searched: 2.5
Enter a valid input!
```
### Result:
Thus, the python program to check the number is Armstrong number or not implemented and the output is verified successfully.

