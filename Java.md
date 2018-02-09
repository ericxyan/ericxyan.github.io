# Java
## Multi-threading
### Locks
#### 

### BlockingQueue
##### Features
A Queue that blocks when you try to dequeue from it and the queue is empty, or if you try to enqueue items to it while the queue is already full.

##### Use Cases
Producer-Consumer pattern

##### Usage
|           |   Throw Exception |   Special Value   |   Block   |           Timeout         |
|-----------|-------------------|-------------------|-----------|---------------------------|
|   Insert  |   add(o)          |   offer(o)        |   put(o)  |   offer(o, time, unit)    |
|   Remove  |   remove(o)       |   poll()          |   take()  |   poll(time, unit)        |
|   peek    |   element()       |   peek()          |           |                           |

##### Exceptions

##### Implementation

### Deadlock
#### Condition

## Heartbeat Mechanism
Source: Oracle JDM Kit 5.0 Heartbeat Mechanism
