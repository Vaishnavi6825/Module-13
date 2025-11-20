# Ex.No: 13C
## POSTFIX EVALUATION
# AIM
To write a Python program to evaluate a user-given Postfix expression that contains Multiplication and Addition operators using the stack concept.

# ALGORITHM
1.Start the program.

2.Define a set named OPERATORS containing all the valid operators: *, +, **, -, /, %.

3.Define a function evaluate_postfix(exp) to evaluate the postfix expression:
4.Inside the function, create an empty list called stack to store operands and intermediate results.

5.Loop through each item in the given postfix expression:
6.If the current item is not in OPERATORS, it is an operand, so append it to the stack.

7.If the current item is an operator:
8.Pop the top two elements from the stack (first pop is a, second pop is b).

9.Perform the operation b <operator> a depending on the current operator.

10.Store the result in a variable called result.

11.Append the result back to the stack.

12.After the loop ends, return the first element of the stack as the final evaluation result.

13.Take a postfix expression as input from the user.

14.Print the postfix expression.

15.Call the function evaluate_postfix() with the input and print the result.

16.End the program.

# PROGRAM
```
# REGNO:-212222060121
# Name:-Kiruthika M
OPERATORS=set(['*','+']) 
def evaluate_postfix(expression):
    stack=[]
    for i in expression:
        if i not in OPERATORS:
            stack.append(i)
        else:
            a=stack.pop()
            b=stack.pop()
            if i=='+':
                res=int(b)+int(a)
            elif i=="*":
                res=int(b)*int(a)
            stack.append(res)
    return stack[0]
expression=input()
print("postfix expression: ",expression)
print("Evaluation result: ",evaluate_postfix(expression))
```

# OUTPUT
<img width="760" height="207" alt="image" src="https://github.com/user-attachments/assets/a2eac34a-4b55-4f73-8830-2c6fcdc38623" />


### RESULT 
Thus a Python program to evaluate a user-given Postfix expression that contains Multiplication and Addition operators using the stack concept has been executed successfully.
