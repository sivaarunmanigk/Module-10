#  Types of Queue-Circular Queue in Python

This project demonstrates the implementation of a **Circular Queue** in Python. The queue accepts 3 user values, performs enqueue and dequeue operations, and displays the removed values.

---

##  Aim

To develop a Python program that implements a Circular Queue:
- Accepts 3 values from the user
- Removes the 3 values from the queue
- Displays the removed values

---

##  Algorithm

1. **Initialize** a circular queue of fixed size (e.g., 5).
2. **Define the following functions**:
   - `enqueue()`: Inserts an element into the queue.
   - `dequeue()`: Removes an element from the queue.
   - `display()`: Shows the queue contents.
3. Accept 3 values from the user using the `enqueue()` method.
4. Remove 3 values using the `dequeue()` method.
5. Print the removed values.

---

##  Program:

```python

class MyCircularQueue:
    def __init__(self, k): self.k, self.q, self.h, self.t = k, [None]*k, -1, -1
    def enqueue(self, v):
        if (self.t + 1) % self.k == self.h: return
        if self.h == -1: self.h = self.t = 0
        else: self.t = (self.t + 1) % self.k
        self.q[self.t] = v
    def printQ(self):
        if self.h == -1: return
        i = self.h
        while i != self.t: print(self.q[i], end=" "); i = (i + 1) % self.k
        print(self.q[self.t])

obj = MyCircularQueue(5)
for _ in range(5): obj.enqueue(int(input()))
obj.printQ()
``` 

### Output:

![image](https://github.com/user-attachments/assets/f4d6dbc0-2f2b-4110-9077-71c20d82c5d6)

## Result:

Thus, the program has been execueted successfully.
