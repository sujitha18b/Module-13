# Exp.No: 13C
## POSTFIX EVALUATION



### AIM  
To write a Python program to evaluate a user-given Postfix expression that contains Multiplication and Addition operators using the stack concept.



### ALGORITHM

1. **Start the program.**
2. Define a set named `OPERATORS` containing all the valid operators: `*, +, **, -, /, %`.
3. Define a function `evaluate_postfix(exp)` to evaluate the postfix expression:
   - Inside the function, create an empty list called `stack` to store operands and intermediate results.
4. Loop through each item in the given postfix expression:
   - If the current item is **not in OPERATORS**, it is an operand, so append it to the stack.
   - If the current item is an **operator**:
     - Pop the top two elements from the stack (first pop is `a`, second pop is `b`).
     - Perform the operation `b <operator> a` depending on the current operator.
     - Store the result in a variable called `result`.
     - Append the result back to the stack.
5. After the loop ends, return the first element of the stack as the final evaluation result.
6. Take a postfix expression as input from the user.
7. Print the postfix expression.
8. Call the function `evaluate_postfix()` with the input and print the result.
9. **End the program.**



### PROGRAM

OPERATORS=set(['*','-','+','%','/','**'])  <br />


def evaluate_postfix(expression):  <br />
    stack=[]  <br />
    for C in expression: <br />
        if C not in OPERATORS: <br />
            stack.append(int(C)) <br />
            stack.append(int(C)) <br />
        else:  <br />
            second = stack.pop()  <br />
            first  = stack.pop()  <br />
            if C == '+':  <br />
                res = int(first)+int(second)  <br />
            elif C == '-':  <br />
                res = int(first)-int(second) <br />
            elif C == '*':  <br />
                res = int(first)*int(second)  <br />
            elif C == '%': <br />
                res = int(first)%int(second) <br />
            elif C == '/':  <br />
                res = int(first)/int(second)  <br />
            elif C == '**':  <br />
                res = int(first)**int(second)  <br />
            stack.append(res) <br />
    return stack[0] <br />



expression = input()  <br />
print("postfix expression: ",expression)  <br />
print("Evaluation result: ",evaluate_postfix(expression))

### OUTPUT
![Screenshot 2025-05-07 104127](https://github.com/user-attachments/assets/325c9d0e-6a95-4cbb-9c8f-bb2df92eddc7)


### RESULT
Thus, the given python program is implemented and executed sucessfully.
