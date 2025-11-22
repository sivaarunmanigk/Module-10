# Queue-Remove Two String Values from the Rear End in Python 

This Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

##  Aim

To write a Python program to:
- Accept `n` string values from the user
- Remove the last two values (rear end of the list)
- Display the updated list

##  Algorithm

1. Create an empty list `q`.
2. Read an integer `n` from the user (number of strings).
3. Loop `n` times:
   - Read a string input.
   - Append it to the list `q`.
4. Remove the last element using `pop()`.
5. Remove the next last element using `pop()` again.
6. Display the updated list.

##  Program:

```python
n=int(input())
l=[]
for i in range(n):
    x=input()
    l.append(x)
l.pop(0)
l.pop(0)
print(f"deque({l})")

```

### Output:

![image](https://github.com/user-attachments/assets/3bf64334-251b-4dfa-93d6-b5dbfced6776)

## Result:

Thus, the program has been successfully executed.
