# op_sys
Projects for CS3013 (Operating Systems) at Worcester Polytechnic Institute C-Term 2016.
The code is not in this repo to prevent cheating in future offerings of the course.
If you are an employer and would like to see my implementations of these projects, please email me at mjgiancola@wpi.edu

## Descriptions

### Project 0

The main purpose of Project 0 was to create a VM in which we created a few new system calls and recompiled the Linux kernel. For now, the system calls just print "Hello World" to the syslog. In project 2, they will do more interesting things.

### Project 1

For this project we developed a simple shell which handles requests by forking processes and using execvp. The final version supports background processes and the "jobs" command.

### Project 2

This project is split into two parts. In the first, we intercept the open, close, and read system calls. We then print information to the syslog about the various calls, including informing the user that their read was malicious if the read buffer contains the word "VIRUS" (a great anti-virus, I know). In the second part, we use the system calls created in Project 0 to implement two different functions. First, the ability to shift a program to a different user ID. The second checks the result of our changes.

### Project 3A

In this project we created our own syncronization problem, akin to the "Dining Philosophers Problem". I wrote a problem for optimizing traffic of swimmers and divers in a swimming pool. I wrote the solution in LaTeX, and compiled it using pdflatex.

### Project 3B

In this project we solved one of the synchronization problems that our peers created in 3A. The problem I solved involved landing 25 lanes onto 3 runways. We solved the problem twice, once using semaphores and once using mutexes / condition variables. The solutions are almost identical except for their use of different synchronization primitives.

### Project 4

In the final project, we implemented a virtual memory system (in user space). Basically, we created an API for accessing memory. The functions of the API allowed a user to create, inspect, modify, and delete pages in memory. Behind the scenes, the API calls handle the eviction of pages between RAM, SSD, and HDD. We were also required to implement 3 different eviction algorithms, one of which uses some notion of history.
