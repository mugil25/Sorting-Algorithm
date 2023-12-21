# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```Python
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Mugil
RegisterNumber: 23008346
'''
def selection_sort(nums):
    for i in range (len(nums)):
        lowest_value_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest_value_index]:
                lowest_value_index=j
        nums[i],nums[lowest_value_index]=nums[lowest_value_index],nums[i]
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
# use the selection sort function
# print the sorted list





```
ii)	#Insertion Sort
```python
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Mugil
RegisterNumber: 23008346
'''
def insertion_sort(nums):
    for i in range(1,len(nums)):
        items_to_insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>items_to_insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=items_to_insert
list_of_nums=eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
   







```

## Output:
1.Write a program to sort the elements in the list using the Selection Sort algorithm.
![image](https://github.com/mugil25/Sorting-Algorithm/assets/148515771/570e0cbd-0471-400f-84e9-36e38e7b0b77)


2.Write a program to sort the elements in the list using the Insertion Sort algorithm.
![image](https://github.com/mugil25/Sorting-Algorithm/assets/148515771/62598798-95aa-4a0f-9e8a-676ce37cbe2b)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
