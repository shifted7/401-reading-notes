Reading 05: Linked Lists

##  Code Fellows: Linked Lists

### What is a Linked List
- A series of `Nodes` connected to each other
  - Each `Node` references the next `Node` in the link
- Two types: Singly and Doubly
  - Focus on Singly Linked List for now
### Terminology:
- Linked List: A data structure that contains nodes that link/point to the next node in the list
- Singly: The nodes have only one reference, and the reference points to the `Next` node in a linked list
- Doubly: The nodes have two references, and those references point to both the `Next` and `Previous` node
- Node: The individual items/links that live in a linked list. Each node contains the data for each link
- Next: Each node contains a property called `Next`. This property contains the reference to the next node
- Head: The head is a reference type of type `Node` to the first node in a linked list
- Current: The `Current` reference is a reference type of type `Node` that is currently being looked at. Traditionally used when traversing through a full linked list. Typically you reset the current to the head to guarantee you are starting from the beginning of the linked list.

### What does it look like

![Linked List](https://github.com/shifted7/401-reading-notes/blob/master/img/image.png)

#### Traversal
- Can't use foreach or for
- We use the `Next` value on each node
- Should use a while loop
  - Check the next node to make sure it is not null
    - If we try to go to it, we'll get a nullreferenceexception and our program will crash
  - The current node is the most helpful
- Ex: Checking whether our linked list includes a value

```
		ALGORTIHM Includes (value)
		// INPUT <-- integer value
		// OUTPUT <-- boolean
			
			Current <-- Head

			WHILE Current is not NULL
				IF Current.Value is equal to value
					return TRUE

				Current <-- Current.Next

			return FALSE
```
#### Adding a Node
```
ALGORITHM Add(newNode)
		// INPUT <-- Node to add 
		// OUTPUT<-- No output

			Current <-- Head
			newNode.Next <-- Head
			Head <-- newNode
			Current <-- Head
```

### Prerequisites
- When making your node class, should require each node has a value
- When making the list, you should require that at least one node gets passed in, to be the head and current.
