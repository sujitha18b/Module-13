# Exp.No:13 D 
## PREFIX EVALUATION


### AIM  
To write a Python program to evaluate a user-given Prefix expression using a stack. The expression must contain operators such as Multiplication, Addition, and Subtraction.



### ALGORITHM

1. **Start the program.**
2. Define a set of valid operators: `*, -, +, %, /, **`.
3. Initialize an empty stack.
4. Traverse the prefix expression from **right to left**:
   - If the character is a **digit**, convert it to an integer and push it onto the stack.
   - If the character is an **operator**, pop two elements from the stack.
     - Apply the operator on the two popped operands.
     - Push the result back onto the stack.
   - If an invalid character is encountered, raise an error.
5. After traversal, the stack should contain only **one element**.
6. Return the **single element** as the evaluation result.
7. **End the program.**



### PROGRAM

OPERATORS=set(['*','-','+','/'])  <br />

def evaluate(expression): <br />

 stack = [] <br />
    for c in expression[::-1]: <br />
        if c not in OPERATORS: <br />
            stack.append(int(c)) <br />
        else: <br />
            o1=stack.pop()  <br />
            o2=stack.pop()  <br />
        if c=='+':  <br />
            stack.append(o1+o2)  <br />
        elif c=='-':  <br />
            stack.append(o1-o2)  <br />
        elif c=='*':  <br />
            stack.append(o1*o2)  <br />
        elif c=='/':  <br />
            stack.append(o1/o2)  <br />
    return stack.pop()  <br />
test_expression=input()  <br />
print("Prefix Expression :",test_expression)  <br />
print("Evaluation result :",evaluate(test_expression))  <br />


### OUTPUT

 ![Screenshot 2025-05-07 104907](https://github.com/user-attachments/assets/c94ece2b-4943-4167-b56a-43b7e10c8d61)



### RESULT
Thus, the given python program is implemented and executed sucessfully.
