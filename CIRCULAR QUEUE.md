# Exp No: 14b 
## Circular Queue - Implementation of Priority Queue Using Python

### AIM  
To implement a priority queue where elements are dequeued based on priority (highest value first) using a Python list and demonstrate insertion, deletion, and traversal operations.
### ALGORITHM
```
1.Initialize an empty list queue to store elements.
2.Define a class PriorityQueue with methods:
      ->isEmpty(): Check if the queue is empty.
      ->insert(data): Add a new element to the queue.
      ->delete():
             ->Find the element with the highest value (highest priority).
             ->Remove it from the queue and return it.
3.Input the number of elements n.
4.Insert elements into the priority queue using insert().
5.Print the queue to display its current state.
6.While the queue is not empty, repeatedly delete the element with the highest priority and print it.
```
### PROGRAM

```
class PriorityQueue(object):
	def __init__(self):
		self.queue = []
	def __str__(self):
		return ' '.join([str(i) for i in self.queue])
	# for checking if the queue is empty
	def isEmpty(self):
		return len(self.queue) == 0
	# for inserting an element in the queue
	def insert(self, data):
		self.queue.append(data)
	# for popping an element based on Priority
	def delete(self):
		try:
			max_val = 0
			for i in range(len(self.queue)):
				if self.queue[i] > self.queue[max_val]:
					max_val = i
			item = self.queue[max_val]
			del self.queue[max_val]
			return item
		except IndexError:
			print()
			exit()
myQueue = PriorityQueue()
n=int(input())	
for i in range(0, n):
    ele = int(input())
    myQueue.insert(ele)
print(myQueue)		
while not myQueue.isEmpty():
	print(myQueue.delete())

```

### OUTPUT
<img width="1180" height="455" alt="image" src="https://github.com/user-attachments/assets/2b89231b-ecb5-41bc-8b31-915631e9fc9d" />


### RESULT
->The program successfully inserts elements into the priority queue.

->The delete() operation removes and returns elements in descending order of priority.

->The program demonstrates the priority-based removal of elements effectively.
