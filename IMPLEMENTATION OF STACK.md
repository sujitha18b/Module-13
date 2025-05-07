# Exp.No: 13B
## IMPLEMENTATION OF STACK


### AIM  
To write a Python program to implement a stack using a list and its built-in methods (`append()`, `pop()`).



### ALGORITHM

1. **Start the program.**
2. **Define a class `st`** with the following methods:
   - `push(self, num)`: Adds the number `num` to the stack.
   - `pop(self)`: Removes and returns the top element from the stack.
3. **Create a stack object `s`** using the class `st`.
4. **Input the stack size**: Take an integer input `size` to define the size of the stack.
5. **Loop through numbers from 1 to size**: Add only the odd numbers to the stack using the `push()` method.
6. **Display the elements** in the stack after the loop completes.
7. **Call `pop()`** to remove the top element from the stack and display the popped element.
8. **Display the stack again** to show the remaining elements.
9. **End the program.**



### PROGRAM

stack = []   <br />
for i in range(7):  <br />
    a=input()  <br />
    stack.append(a)  <br />

print('Stack before elements are popped')  <br />
print(stack)  <br />

for i in range(5): <br />
    stack.pop() <br />


print('\nStack after elements are popped:') <br />
print(stack)

### OUTPUT
![Screenshot 2025-05-07 103726](https://github.com/user-attachments/assets/8c8fefd0-5184-437e-978c-dcfc7c973c0d)

### RESULT
Thus,the given python program is implemented and sucessfully.
