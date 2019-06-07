**1. List all of the main states a process may be in at any point in time on a standard Unix system. Briefly explain what each of these states means.**
-Created: When a process is first created, it occupies the "created" or "new" state.
-Ready: A "ready" or "waiting" process has been loaded into main memory and is awaiting execution on a CPU.
-Running: A process moves into the running state when it is chosen for execution.
-Blocked: A process transitions to a blocked state when it cannot carry on without an external change in state or event occurring.
-Terminated: A process may be terminated, either from the "running" state by completing its execution or by explicitly being killed.

**2. What is a zombie process?**
A zombie process is a process that has been completed, but still has entry in the process table.

**3. How does a zombie process get created? How does one get destroyed?**
Zombie processes are created when a process, usually a child oone, is done executing and is waiting on termination from the parent. Until the parent is done and can clean up the child, it is a zombie.

**4. What are some of the benefits of working in a compiled language versus a non-compiled language? More specifically, what benefits are there to be had from taking the extra time to compile our code?**
One of the main benefits of compiled language is the fast performance. Because there is hardly any abstraction at all, many of the executions are fed directly into the machine without hardly any middlemen doing work. On the other hand, using a non-compiled language gives you the convenience of abstraction, and is much easier to implement. However because you rely on so many processes, the code is often not as performant.
