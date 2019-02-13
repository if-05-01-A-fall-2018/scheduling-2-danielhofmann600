### if.05.01 TINF Operting Systems

# Assignment 8: Scheduling
## Objective
The goal of this week's assignment is to deal with scheduling of interactive and real time systems.

## Required Tasks
Answer the following questions

1. **Multiple Queues**
A process on a system with Multiple Queues Scheduling needs 30 quanta to complete. How many times must it be swapped in, including the very first time (before it has run at all)?

		It needs to swap 5 times.

2. **Shortest Process Next**
A scheduler working with the {\em Shortest Process Next} Strategy has two processes in ready state and has to schedule one of these:

| Process Name | 1st run | 2nd run | 3rd run | 4th run |
| -- | -- | -- | -- | -- |
A | 50 msec | 150 msec | 300 msec | 85 msec |
B | 300 msec | 150 msec | 85 msec | 50 msec

Which process will be taken by the scheduler and why?

		A: 142,5
		B: 102,5 -> in conclusion the Sheduler takes Procces B first

3. **CPU-bound and I/O-bound Processes**
	- Explain in a few words the terms CPU-bound and I/O-bound processes.
	- Why is it important for the scheduler to distinguish between CPU-bound and I/O-bound processes?

			An CPU-boud Process needs more Quantas time to finish but doesn't need to be called that often.  
			An IO-bound Process has to wait on User Input and therefore needs to be called more aften but doesn't need as many quantas. 

4. **Real Time Schedulable**
A soft real-time system has four periodic events with periods of 50, 100, 200, and 250 msec each. Suppose that the four events require 35, 20, 10 and $x$ msec of CPUtime, respectively. What is the largest value of $x$ for which the system is schedulable?

		Σ Ci/Pi <= 1

		35 / 50 + 20 / 100 + 10 / 200 + $x$ / 250 <= 1 

		0,7 + 0,2 + 0,05 + $x$ / 250 <= 1

		0,95 + $x$ / 250 <= 1

		$x$ / 250 <= 0,05

		$x$ <= 12,5
