# # Stack-Stack Reversal Program 🔁

This Python program demonstrates how to reverse the values in a stack using basic stack operations like push and pop.

## 🎯 Aim

To write a Python program that reverses the values in a stack using standard stack operations.

## 📋 Algorithm

1. Create an empty stack.
2. Read an integer `n` from the user (number of elements to push).
3. Loop `n` times:
   - Read an integer from the user.
   - Push it onto the stack.
4. Create an empty list called `reverse`.
5. While the stack is not empty:
   - Pop the top element.
   - Append it to `reverse`.
6. Print the reversed list.


### Program:

# Reg.No: 212222210020
# Name: Prithisha S

stack = list(map(int, input("Enter stack elements: ").split()))

stack.reverse()

print("Reversed stack:", stack)

## 🧪 Output

Enter stack elements: 1 2 3 4
Reversed stack: [4, 3, 2, 1]

## Result
The programs were implemented successfully and the outputs were verified.
