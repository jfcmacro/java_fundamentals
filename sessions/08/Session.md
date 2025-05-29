# Session 08 - Java Concurrent Essentials

Agenda:

* Introduction to Java threads
* The concepts of concurrency and parallelism
* Creating and starting threads in Java
* Synchronization in Java threads
* Race conditions and data hazards
* Thread lifecycle: states and transitions
* Thread synchronization using locks and monitors
* Thread safety and atomic operations
* Thread interruption and termination
* Thread Factory (Task)
* Concurrent TicTacToe (Task)

---

# Introduction to Java threads

- What are threads and their importance in Java?
- Differences between processes and threads
- Multithreading benefits and use cases
- Java Thread class and Runnable interface

---

# The concepts of concurrency and parallelism

* Understanding concurrency and parallelism

- Concurrent vs parallel execution
- Benefits and challenges of concurrent programming

---

# Creating and starting threads in Java

- Extending the Thread class
- Implementing the Runnable interface
- Starting threads using start() method
- Thread naming and identification

---

## Java Threads

* `Thread` class
* `Runnable`
* Implementation

---

# Synchronization in Java threads

- Understanding synchronization and its purpose
- Critical sections and mutual exclusion
- Thread interference and memory consistency errors
- Using synchronized blocks and method

---

## Java Synchronization Primitives

* `synchronized` methods
* `synchronized` blocks
* `wait` methods
* `notify` and `notifyAll` methos

---

# Thread lifecycle: states and transitions

- Thread states: new, runnable, blocked, waiting, timed waiting, terminated
- Transition between states
- Thread sleep and join methods

---

# Thread synchronization using locks and monitors

- Lock objects and their usage
- Reentrant locks and fairness policies
- Condition variables and signaling

---

# Thread safety and atomic operations

- Thread safety concepts and importance
- Atomic variables and their usage
- Atomic operations and their guarantees

---

# Thread interruption and termination

- Interrupting threads
- Handling thread interruption
- Graceful thread termination

---

# Thread Factory (Task)

* [Description](https://gitlab.com/juan_cardona_epam/thread-factoring)


## Concurrent TicTacToe (Task)

* [Description](https://gitlab.com/juan_cardona_epam/concurrent-tic-tac-toe)


