# Exp.No:31
# IMPLEMENTATION OF STACK
# AIM
To write a Python program to implement a stack using a list and its built-in methods (append(), pop()).

# ALGORITHM
1.Start the program.

2.Define a class st with the following methods:
push(self, num): Adds the number num to the stack.

3.pop(self): Removes and returns the top element from the stack.

4.Create a stack object s using the class st.

5.Input the stack size: Take an integer input size to define the size of the stack.

6.Loop through numbers from 1 to size: Add only the odd numbers to the stack using the push() method.

7.Display the elements in the stack after the loop completes.

8.Call pop() to remove the top element from the stack and display the popped element.

9.Display the stack again to show the remaining elements.

10.End the program.

# PROGRAM
```
# REGNO:-212222060121
# name:-Kiruthika M
stack = []
for i in range(5):
    s=input()
    stack.append(s)
print("Stack before elements are popped")
print(stack)
stack.pop()
stack.pop()
print("\nStack after elements are popped:")
print(stack)
```

# OUTPUT
<img width="1226" height="557" alt="image" src="https://github.com/user-attachments/assets/4cee64e8-b817-4824-85a0-2f15a7db7845" />


# RESULT
Thus a Python program to implement a stack using a list and its built-in methods (append(), pop()) has been executed succesfully.
