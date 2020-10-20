# Class 10 \| Implementation: Stacks and Queues
Article: [Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)     
 
## Notes on Stacks & Queues reading from CF
- Stack is the data structure of nodes which reference other nodes in the "stack", think vertical
- Queue is similiar to stack but horizontal, and a place where things que up to be pushed onto the stack

> Both models follow FIFO(first in first out) & LILO(last in last out) flow

- There are 2 key terms both flows share which are: `peek` and `isEmpty`. 
  - With `peek` you are looking at the "first" node, so for stack it's the `top` node and for queue it's the `front` node to be specific
  - When you `peek` on either, you're peeking at the top or front node respectively
  - `isEmpty` returns boolean `true` when the queue or stack is empty

- All the key terms take BigO O(1) since they take the same amount of time no matter how many nodes are in the stack or queue

> Stack Terms  
> - Push | a node put into the stack
> - Pop | a node removed from the stack
> - Top | the node on the top of the stack
> - Peek (see above)  
> - isEmpty (see above)  

> Queue Terms  
> - Enqueue | a node added to the que
> - Dequeue | a node removed from que
> - Front | the first node of the que
> - Rear | the last node of the que
> - Peek (see above)  
> - isEmpty (see above) 



[Back to Home](README.md)