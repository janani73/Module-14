# Exp.No:14c
## DEQUE - Implementation of Double-Ended Queue (Deque) Using Python collections Module
### AIM  
To demonstrate the use of a deque for adding elements at the right end and displaying the updated deque.
### ALGORITHM  
```
1.Import the collections module to use the deque class.
2.Input three initial elements from the user (n1, n2, n3).
3.Create a deque with the input elements: deque([n1, n2, n3]).
4.Append additional elements 'h', 'o', and 'n' to the right end of the deque using append().
5.Print the deque to display all current elements after the append operations.
```
### PROGRAM  

```
import collections
n1=input()
n2=input()
n3=input()
de=collections.deque([n1,n2,n3])
de.append('h')
de.append('o')
de.append('n')
print("The deque after appending at right is :")
print(de)
```

### OUTPUT
<img width="1172" height="237" alt="image" src="https://github.com/user-attachments/assets/691c7910-ce67-4369-8438-696eec65d962" />

### RESULT
->The program creates a deque with initial elements.

->Additional elements are successfully appended to the right end.

->The final deque reflects the updated sequence of elements.
