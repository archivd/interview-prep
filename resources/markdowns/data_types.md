Here's a practical guide for Java's main DSA data types: **Stack**, **Queue**, **Deque**, and **Heap**. For each, I'll cover how to create them, insert/add elements, access elements, and perform basic operations, along with concise code examples.

***

## 1. Stack

A Stack is a LIFO (last-in, first-out) structure.

**Creating:**
```java
import java.util.Stack;
Stack stack = new Stack<>();
```

**Basic operations:**
```java
stack.push(10);             // Insert
stack.push(20);
int top = stack.peek();     // Read top element (no removal)
int removed = stack.pop();  // Remove top element
boolean isEmpty = stack.isEmpty();

for(Integer item : stack) { // Iterate
    System.out.println(item);
}
```
- `.push(x)`: Adds to TOP.
- `.pop()`: Removes and returns TOP.
- `.peek()`: View TOP without removal.
- `.isEmpty()`: Checks if stack is empty.
- Iteration visits bottom to top.[1][2]

***

## 2. Queue

A Queue is FIFO (first-in, first-out). Use `LinkedList` or `ArrayDeque`:

**Creating:**
```java
import java.util.Queue;
import java.util.LinkedList;

Queue queue = new LinkedList<>();
```

**Basic operations:**
```java
queue.offer(10);                // Insert at rear
queue.offer(20);
int front = queue.peek();       // Read front element (head), doesn't remove
int removed = queue.poll();     // Remove and return front
boolean isEmpty = queue.isEmpty();

for(Integer item : queue) {     // Iterate front to rear
    System.out.println(item);
}
```
- `.offer(x)`: Add to rear.
- `.poll()`: Remove front.
- `.peek()`: See front.
- `.isEmpty()`: Empty?
- You can also use `ArrayDeque` for better performance.[3]

***

## 3. Deque (Double-Ended Queue)

Elements can be inserted/removed at both ends.

**Creating:**
```java
import java.util.Deque;
import java.util.ArrayDeque;

Deque deque = new ArrayDeque<>();
```

**Basic operations:**
```java
deque.addFirst(1);            // Insert at front
deque.addLast(10);            // Insert at rear
int first = deque.peekFirst(); // Front element
int last = deque.peekLast();   // Rear element

deque.removeFirst();          // Remove from front
deque.removeLast();           // Remove from rear

for(Integer item : deque) {   // Iterate front to rear
    System.out.println(item);
}
```
- `.addFirst(x)`, `.addLast(x)`
- `.removeFirst()`, `.removeLast()`
- `.peekFirst()`, `.peekLast()`.[3]

***

## 4. Heap (Priority Queue)

Min-Heap by default. (For max-heap, use a custom comparator).

**Creating:**
```java
import java.util.PriorityQueue;

PriorityQueue minHeap = new PriorityQueue<>(); // Min-heap
PriorityQueue maxHeap = new PriorityQueue<>((a, b) -> b - a); // Max-heap
```

**Basic operations:**
```java
minHeap.offer(5);
minHeap.offer(2);
minHeap.offer(8);

int min = minHeap.peek();      // Root element (smallest)
int removed = minHeap.poll();  // Remove root

for(Integer item : minHeap) {  // No particular order!
    System.out.println(item);
}
```
- `.offer(x)`: Add
- `.peek()`: See root/min
- `.poll()`: Remove root
- Iteration does not give sorted output!
- For custom objects, supply a comparator.

***

### Notes on Arrays and Strings

- Arrays and Strings are basic types. Declaration:
```java
int[] arr = new int[11];
arr = 10;                  // Access/set by index
for(int i = 0; i < arr.length; i++) { ... }
```

- Strings
```java
String s = "hello";
char first = s.charAt(0);     // Access by index
for(char c : s.toCharArray()) { ... }
```

- Summary Table

| Data Type | Create                | Add                      | Access                   | Remove                       | Iterate                    |
|-----------|-----------------------|--------------------------|--------------------------|------------------------------|----------------------------|
| Stack     | new Stack<>()         | .push(x)                 | .peek()                  | .pop()                       | for-each loop              |
| Queue     | new LinkedList<>()    | .offer(x)                | .peek()                  | .poll()                      | for-each loop              |
| Deque     | new ArrayDeque<>()    | .addFirst(x),.addLast(x) | .peekFirst(),.peekLast() | .removeFirst(),.removeLast() | for-each                   |
| Heap      | new PriorityQueue<>() | .offer(x)                | .peek()                  | .poll()                      | for-each (order arbitrary) |

<br><br>
With these code snippets and explanations, you willll be able to create, use, and operate on stacks, queues, deques, and heaps in Java with confidence.[4][2][3]

[1] https://www.codecademy.com/resources/docs/java/stack<br>
[2] https://www.educative.io/answers/how-to-use-the-stack-class-in-java<br>
[3] https://www.educative.io/answers/queue-vs-deque-in-java<br>
[4] https://www.sanfoundry.com/java-program-implement-heap/<br>
[5] https://www.geeksforgeeks.org/java/stack-class-in-java/<br>
[6] https://www.programiz.com/java-programming/stack<br>
[7] https://www.baeldung.com/java-stack<br>
[8] https://zerotomastery.io/blog/stack-memory-in-java-beginners-guide/<br>
[9] https://www.geeksforgeeks.org/dsa/difference-between-queue-and-deque-queue-vs-deque/<br>
[10] https://www.programiz.com/dsa/heap-data-structure<br>
[11] https://www.coursera.org/articles/types-of-data-structures<br>
