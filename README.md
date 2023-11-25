# Calculate-the-sum-of-elements-in-an-array-using-Python


Methods Discussed in this page are :
Method 1 : Using Iteration
Method 2 : Using recursion
Method 3 : Using inbuilt Function
Method 1 :
Declare a variable say Sum =0 to hold the value of sum
Run a loop for range( len(arr))
Set variable Sum = Sum + arr[i]
After complete iteration print value Sum
Method 1 : Python Code
Run
arr = [10, 89, 9, 56, 4, 80, 8]
Sum = 0

for i in range(len(arr)):
   Sum = Sum + arr[i]
print (Sum)
Output
256
Related Pages
Find the Smallest and largest element in an array

Find Second Smallest Element in an Array

Reverse an Array

Sort first half in ascending order and second half in descending 

Sort the elements of an array

Method 2 :
Create a recursive function say getSum(arr, n)
Base Condition : if(n==0) then return 0
Otherwise, return arr[n-1] + getSum(arr, n-1)
Method 2 : Python Code
Run
def getSum(arr, n):
   if n == 0:
     return 0
   return arr[n-1] + getSum(arr, n-1)
arr = [10, 20, 30, 40]
print(getSum(arr, len(arr)))
Output
100
Method 3:
Using in-built function sum(arr), we can get the sum of the elements of the array passed to it.
Method 3 : Python Code
Run
arr = [10, 20, 30, 40]
print(sum(arr))
Output
100
