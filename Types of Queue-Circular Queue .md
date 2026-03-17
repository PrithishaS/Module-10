# 🔄 Types of Queue-Circular Queue in Python

This project demonstrates the implementation of a **Circular Queue** in Python. The queue accepts 3 user values, performs enqueue and dequeue operations, and displays the removed values.

---

## 🎯 Aim

To develop a Python program that implements a Circular Queue:
- Accepts 3 values from the user
- Removes the 3 values from the queue
- Displays the removed values

---

## 🧠 Algorithm

1. **Initialize** a circular queue of fixed size (e.g., 5).
2. **Define the following functions**:
   - `enqueue()`: Inserts an element into the queue.
   - `dequeue()`: Removes an element from the queue.
   - `display()`: Shows the queue contents.
3. Accept 3 values from the user using the `enqueue()` method.
4. Remove 3 values using the `dequeue()` method.
5. Print the removed values.

---

## 💻 Program:
# Reg.No: 212222210020
# Name: Prithisha S

class CircularQueue:
    def __init__(self, size):
        self.queue = [None]*size
        self.size = size
        self.front = self.rear = -1
    def insert(self, data):
        if (self.rear + 1) % self.size == self.front:
            print("Queue is Full")
        elif self.front == -1:
            self.front = self.rear = 0
            self.queue[self.rear] = data
        else:
            self.rear = (self.rear + 1) % self.size
            self.queue[self.rear] = data

   def display(self):
        print("Queue:", self.queue)

cq = CircularQueue(3)
cq.insert(1)
cq.insert(2)
cq.insert(3)
cq.display()

### Output:

Queue: [1, 2, 3]

## Result:
The programs were implemented successfully and the outputs were verified.
