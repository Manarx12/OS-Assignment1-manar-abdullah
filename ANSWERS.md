# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

A Process is an independent program in execution that has its own memory space and resources. A Thread, however, is a smaller unit of execution within a process that shares the same memory space as other threads in that process.

Differences: Creating a process has high overhead and consumes more memory, while threads are "lightweight" and share resources, making communication between them much faster.

Why threads in this assignment?: We used threads because they are more suitable for simulating a CPU scheduler within a single application. It allows us to manage multiple "tasks" (processes) efficiently without the heavy overhead of creating entirely separate operating system processes.

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**
In Round-Robin scheduling, if a process does not finish its execution within the given Time Quantum, it is preempted. The CPU saves its state, and the process is moved to the back of the Ready Queue to wait for its next turn.

Example from my output:
```
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example:**
In this snippet, P1 had a burst time that was longer than the 100ms quantum. After executing for 100ms, it still had 100ms remaining. Therefore, the scheduler paused P1, moved it to the end of the queue, and switched to the next available process to ensure fairness.

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

Trace of process P1 through its lifecycle:

New: When the Process object is instantiated in the code but the thread hasn't started yet.

Runnable: When the process is added to the processQueue and is waiting for its turn to be picked by the scheduler.

Running: When the scheduler calls currentThread.start(), and P1 is actually executing its run() method on the CPU.

Waiting/Blocked: In this simulation, this happens during Thread.sleep(), where P1 "waits" to simulate the passage of time for its burst execution.

Terminated: When remainingTime reaches 0 and the run() method completes, the thread finishes its execution.



## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

Example 1: Web Servers (Handling multiple requests)
Description: A web server receiving hundreds of requests from different users at the same time.
Why Round-Robin works well: It ensures that no single user has to wait too long. Every request gets a small slice of CPU time, providing good responsiveness and fairness for all connected users.

Example 2: Time-Sharing Operating Systems
Description: Multiple users or applications running on a single computer (like a lab computer).
Why Round-Robin works well: It prevents a single heavy application (like a video editor) from freezing the entire system. By giving every app a quantum, the system remains interactive for the user.

## Summary

**Key concepts I understood through these questions:**
The efficiency of using Threads for multitasking within a single program.

The importance of the Time Quantum in balancing fairness and performance.

The lifecycle of a thread and how it moves between different states during execution.

**Concepts I need to study more:**
1. 
2. 
