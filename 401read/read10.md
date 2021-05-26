# Stacks and Queues

## Stack 

In the pushdown stacks only two operations are allowed: push the item into the stack, and pop the item out of the stack. A stack is a limited access data structure - elements can be added and removed from the stack only at the top. push adds an item to the top of the stack, pop removes the item from the top. A helpful analogy is to think of a stack of books; you can remove only the top book, also you can add a new book on the top.

![STACK](https://res.cloudinary.com/practicaldev/image/fetch/s--s1Qbl8Gf--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/mwcwre09s12vqa3gvl7a.png)

### Common terminology for a stack is

- `Push` - Nodes or items that are put into the stack are pushed
- `Pop` - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
- `Top` - This is the top of the stack.
- `Peek` - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
- `IsEmpty` - returns true when stack is empty otherwise returns false.


## Queue 

 New additions to a line made to the back of the queue, while removal (or serving) happens in the front. In the queue only two operations are allowed `enqueue` and `dequeue`.
 
  Enqueue means to insert an item into the back of the queue, dequeue means removing the front item. The picture demonstrates the FIFO access.
  
   The difference between stacks and queues is in removing. In a stack we remove the item the most recently added; in a queue, we remove the item the least recently added.

![Queue](https://i0.wp.com/learnersbucket.com/wp-content/uploads/2019/01/Queue-2-1.png?fit=768%2C400&ssl=1)



### Common terminology for a queue is

- `Enqueue` - Nodes or items that are added to the queue.
- `Dequeue` - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
- `Front` - This is the front/first Node of the queue.
- `Rear` - This is the rear/last Node of the queue.
- `Peek` - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
- `IsEmpty` - returns true when queue is empty otherwise returns false.


## FIFO & LILO and LIFO & FILO Principles
- Queue: **First In First Out (FIFO)**: The first object into a queue is the first object to leave the queue, used by a queue.

- Stack: **Last In First Out (LIFO)**: The last object into a stack is the first object to leave the stack, used by a stack

OR

- Stack: **Last In First Out (FILO)**: The First object or item in a stack is the last object or item to leave the stack.

- Queue: **Last In First Out (LILO)**: The last object or item in a queue is the last object or item to leave the queue.