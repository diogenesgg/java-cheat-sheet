# java-cheat-sheet
My Notes on Java

## Deprecated Classes/APIs
 - SimpleDateFormat
 - java.util.Date
 - java.util.HashTable
   - Not officially deprecated (with the @Deprecated). However, it is widely considered obsolete, and its use is discouraged for new development.
   - Use HashMap or ConcurrentHashMap instead.

## Multithreading/Concurrency
 - synchronized:
   - When applied to multiple methods, one method being accessed blocks the other synchronized methods!
   - a synchronized block is Reentrant: a thread cannot prevent itself from entering a/another critical section.
 - atomic operations:
   - all reference assignments;
   - all primitive assignments, except for long and double;
- volatile:
   - "This variable changes a lot, and is accessed by multiple threads! Don't cache it at the CPU level (registers, cache), only have it in memory."
   - When applied to double and long primitives, it guarantees their assignment is atomic. 

## Collections Classes
- List
  - ArrayList
  - LinkedList
  - CopyOnWriteArrayList
    - A thread-safe variant of ArrayList in which all mutative operations (add, set, and so on) are implemented by making a fresh copy of the underlying array.
- Map
  - HashMap
  - LinkedHashMap
  - TreeMap
  - ConcurrentHashMap
- Set
  - HashSet
  - LinkedHashSet
  - TreeSet
  - CopyOnWriteArraySet
  - ConcurrentSkipListSet
- Queue
  - PriorityQueue
  - ConcurrentLinkedQueue
  - ArrayBlockingQueue
  - PriorityBlockingQueue
- Deque (insertion and removal at both ends. "double ended queue")
  - LinkedList
  - ArrayDeque
  - ConcurrentLinkedDeque
  - LinkedBlockingDeque
- Heap
  - PriorityQueue
    - PriorityQueue<Integer> minHeap = new PriorityQueue<>();
    - PriorityQueue<Integer> maxHeap = new PriorityQueue<>(Comparator.reverseOrder());
    - add and poll methods
- Stack
  - LinkedList
  - Deque implementations
  - ~Stack~ (extends the obsolete Vector class)

## Virtual Threads
 - 

## Memory Management 
 - Heap vs stack vs metaspace 

## Date and Time
 
## Functional Programming

