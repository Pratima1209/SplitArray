# SplitArray
# Python Program to Split the array and add the first part to the end with user Input


# User Input in Array
arr=[]
a=int(input("Enter the number of Element in Array :"))
for i in range(a):
    arr.append(int(input("Enter the Number:")))
# len of array
n=len(arr)
# split by 1
k=1

# Define function 
def split_Array(arr,n,k):
    for i in range(0,k):
      # Store first element in temp veriable
        temp=arr[0]
        # shift elements by 1
        for j in range(0,n-1):
            arr[j]=arr[j+1]
        # assign temp value in last element
        arr[n-1]=temp

# main to print array
split_Array(arr,n,k)
for i in range(0,n):
    print(arr[i],end="")

