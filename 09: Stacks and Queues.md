# Reading 09: Stacks and Queues

## What is a Stack
- Data structure that uses nodes
  - Each node references the next node
    - Same as linked list
- Common terminology:
  - Push - Nodes or items are put into the stack at the top
  - Pop - Nodes or items are removed from the stack
  - Top - The top of the stack
  - Peek - View the value of the top node of the stack
    - Will raise exception if item is empty
  - IsEmpty - Checks whether the stack is empty, else returns false
  
### FILO
  - First In Last Out
  - First item added to the stack will be last item popped out
  
### LIFO
  - Last In First Out
  - The last item added will be the first item popped out
  
### Stack Visualization
  
  ![The stack](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG)
  
### Push O(1)
  - Takes same amount of time regardless of number of nodes
  
### Pop O(1)
  - removes node from the top
  - Check isEmpty before using a pop
  - Steps: Create temp, assign to top. Reassign top to next. Clear temp.next. Return temp
  
### Peek O(1)
  - Just returns top.value
  
### IsEmpty O(1)
  - Just returns whether top == null
  
## What is a Queue
- Enqueue - Nodes or items are added to the queue
- Dequeue - Nodes or items are removed from the queue (empty = exception)

### FIFO
- First item in the queue will be the first item out

### LILO
- Last item in the queue will be the last item out of the queue

### Queue Visualization
![Queue](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Queue.PNG)

### Enqueue O(1)
- Steps: Change next of rear node to new node. Change rear to new node.

### Dequeue O(1)
- Check isEmpty
- Steps: create temp, assign to front. Assign front to front.next. Clear temp.next.

### Peek
- Same as above

### isEmpty
- Same as above

