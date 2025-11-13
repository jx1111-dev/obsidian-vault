
==PROCESS SCHEDULING==

It consists of:

**Programs**. They are referred to passive entities, texts that don't do anything until executed, An operating system can run it in 3 main different ways:

Batch mode is like jobs. It is a list of jobs (or tasks) that get executed sequentially, one by one.

Real time mode is when programs are attached to a terminal session. Programs can be run in the foreground and background. For example, four windows are open, but only one is responding to user input.

Server mode (or daemon mode for unix) runs continuously while computer is on, waiting for a user to connect.

**Processes**. As opposed to programs, they are active entities. Think about it like a program in execution. It's both more and less than a program, because firstly, it goes beyond the code, and secondly, it can be the same program producing more than one process.

**Interleaving**. This is a process that interleaves the execution of multiple programs to maximise processor utilisation. Think of it as a group of processes asking a CPU for resources.

**Process Control Block (PCB)**. It is a data structure, located in the OS's kernel. It contains all the information required to process scheduling. 

For each process, the OS must store information in the PCB in order to execute the process, save the execution state if interrupted, or restore the execution state and continue.

![[Pasted image 20251111093022.png]]

==SELECTING THE NEXT PROCESS TO EXECUTE ON THE CPU==

It is a fundamental operating system function.  Its goal is to:

Obtain maximum CPU utilisation using multiprogramming.

Allow more than one process to be loaded into the CPU at a time.

Loaded processes use the CPU simultaneously using time plexing.

**Types of process scheduling queues**
The **Job Queue** stores PCBs of all the processes in the system (RAM or on disk)

The **Ready Queue** stores PCBs of processes in RAM, ready and waiting to execute

The **Device queues** stores PCBs of processes waiting for a I/O device (e.g. keyboard mouse blah blah)

![[Pasted image 20251111093612.png]]
![[Pasted image 20251111093640.png]]
![[Pasted image 20251111093656.png]]

**CPU utilisation** means the number of processes that complete their execution per time unit.

**Turnaround time** means the amount of time to execute a particular process.

**Wait time** means the amount of time a process has been waiting in the ready queue.

**Response time** means the amount of time between the moment a request was submitted and the moment the first response is produced.

==PRIORITY==

Priority refers to how the OS decides what processes to execute first. These are the metrics that affect priority:

-CPU requirements.
-I/O requirements.
-Memory requirements.
-Time since last slice of CPU.
-Time priority of user.
-State of I/O devices.

==ALGORITHM EVALUATION==

![[Pasted image 20251111094342.png]]

**Deterministic modelling** takes a predetermined workload and defines the performance of each algorithm for that workload.

**Queuing models** estimate arrival rates and service rates to compute utilisation, average queue length, average wait time, etc.

**Algorithm evaluation** creates a model of a computer system and scheduling algorithms. Draws random data from mathematical models and real system traces to drive the simulation.

**Implementation** implements the algorithm and tries it in the OS.

==PROCESSES AND THREADS==

A thread is a lightweight subprocess. A process can be divided into many threads.

Each thread has its own program counter, register values and stack.

Threads can share code, data and resources with other threads from the same process.

Some systems consider threads to be the fundamental execution unit. 

(think of threads as lanes of a CPU, you can execute a process by dividing it between multiple lanes to increase efficiency, instead of running it all through a single lane. )

