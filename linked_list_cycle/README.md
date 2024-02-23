
# Detecting Cycles in Linked Lists
## What is a Cycle in a Linked List?
A cycle in a linked list occurs when a node's next pointer points to a previously visited node. This creates a loop, making it impossible to reach the end of the list (null terminator).

## How to Spot a Cycle
Cycles can be detected using the Floyd's Tortoise and Hare algorithm, which employs two pointers that move at different speeds through the list. If these pointers ever meet, a cycle exists.

The Hare and Tortoise Algorithm
Tortoise: Moves one step at a time.
Hare: Moves two steps at a time.
If the hare ever catches up to the tortoise (i.e., both pointers point to the same node), a cycle is detected. This method efficiently spots cycles without needing extra memory for tracking visited nodes.