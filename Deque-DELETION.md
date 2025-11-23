# Exp.No:38  
## Deque - Removing Elements from the Right End of a Deque Using Python
### AIM  
To demonstrate the double-ended queue (deque) functionality by removing elements from the right end using the pop() method.
### ALGORITHM  
```
1.Import the collections module to use the deque class.
2.Input three integer elements from the user (n1, n2, n3).
3.Create a deque with the input elements: deque([n1, n2, n3]).
4.Remove the element from the right end using pop().
5.Print the deque to display the current state after removing the element.
```

### PROGRAM  

```
import collections
n1=int(input())
n2=int(input())
n3=int(input())
de=collections.deque([n1,n2,n3])
de.pop()
print(de)
```

### OUTPUT
<img width="1172" height="322" alt="image" src="https://github.com/user-attachments/assets/95e192f0-1907-415c-85a6-026004521e0e" />


### RESULT
->The program initializes a deque with user-provided elements.

->The rightmost element is removed successfully.

->The deque is updated and displayed showing the remaining elements.
