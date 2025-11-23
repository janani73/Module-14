# Exp.No:14e 
## PRIORITY QUEUE - Using Python collections.deque to Insert Elements at the Left End

### AIM  
To demonstrate the deque (double-ended queue) functionality by adding elements at the left end and displaying the updated deque.
### ALGORITHM
```
1.Import the collections module to use the deque class.
2.Input three elements from the user (a, b, c).
3.Create a deque with the input elements: deque([a, b, c]).
4.Append elements 'h', 'o', and 'n' to the left end using appendleft().
5.Print the deque to display the current state after the append operations.
```
### PROGRAM
```
import collections
a=input()
b=input()
c=input()
de=collections.deque([a,b,c])
de.appendleft('h')
de.appendleft('o')
de.appendleft('n')
print("The deque after appending at right is :")
print(de)
```
### OUTPUT
<img width="1195" height="313" alt="image" src="https://github.com/user-attachments/assets/e1ce33ac-6dc0-4ec4-80cd-e5c9dc343e55" />

### RESULT
->The program initializes a deque with the user-provided elements.

->New elements are successfully added to the left end in the order they were appended.

->The final deque reflects the updated order with the leftmost elements appearing first.
