# Exp.No:14a  
## APPLICATIONS OF QUEUE - Implementation of Queue Data Structure Using Python

### AIM  
To implement a queue using Python with basic operations like enqueue, dequeue, check empty, and display, and to demonstrate the FIFO (First-In-First-Out) principle.
### ALGORITHM  
```
1.Initialize a queue with a fixed size (limit) and set front and rear pointers to 0.
2.Define methods in the Queue class:
      ->isempty(): Check if the queue is empty.
      ->enqueue(item):
          ->Check if the queue is full (len(queue) == limit).
          ->If not full, insert the item at the front position and increment front.
      ->dequeue():
          ->Check if the queue is empty.
          ->If not empty, remove the item at the rear position and increment rear.
      ->display(): Show all elements in the queue.
3.Input the queue size and elements to enqueue.
4.Call enqueue() to add elements to the queue.
5.Display the queue using display().
6.Call dequeue() to remove the first element.
7.Display the queue again to show the updated state.
```
### PROGRAM  

```
class Queue:
    def __init__(self,limit):
        self.queue=[]
        self.rear=0
        self.front=0
        self.limit=limit
    def isempty(self):
        if len(self.queue)==0:
            return True
        else:
            return False
    def enqueue(self,item):
        if len(self.queue)==self.limit:
            print("Queue is full")
        else:
            if (self.front)==self.limit:
                self.front=self.rear-1
            self.queue.insert(self.front,item)
            self.front+=1
    def dequeue(self):
        if len(self.queue)==0:
            print("Stack is overflow")
        else:
            if (self.rear)==self.limit:
                self.rear=0
            self.queue.pop(self.rear)
            self.rear+=1
    def display(self):
        float_no=[float(i) for i in self.queue]
        print(float_no)
size=int(input())
a=Queue(size)
n1=int(input())
n2=int(input())
n3=float(input())
a.enqueue(n1)
a.enqueue(n2)
a.enqueue(n3)
a.display()
a.dequeue()
a.display()

```

### OUTPUT
<img width="1172" height="258" alt="image" src="https://github.com/user-attachments/assets/27f52797-d6f1-4b6f-87b3-c4c04fcf4207" />


### RESULT
->The program correctly enqueues and dequeues elements in the queue.

->The display() method shows the current state of the queue in FIFO order.

->The queue handles both integers and float values.
