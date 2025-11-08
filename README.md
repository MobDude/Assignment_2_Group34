# **SYSC4001 - Assignment 2**
### Shared Memory + Semaphore Synchronization and API Simulator (fork/exec)

## Authors:
- Mark Bowerman

## Overview
This assignment is divided into two main parts:

### Part II - Shared Memory and Semaphores

This section demonstrates inter-process communication using shared memory protected by System V semaphores.
Two processes concurrently access and update a shared variable, with semaphore synchronization ensuring mutual exclusion.

Each process:
- Attaches to the same shared memory segment.
- Reads and updates a common integer variable.
- Displays its process ID and current shared variable value.
- Terminates when the shared variable exceeds 500.

Semaphore operations (semget, semop, semctl) protect the shared memory region to avoid race conditions.

### Part III - API Simulator: fork() / exec()

This simulator models a simplified Operating System environment with fixed memory partitions, a process control block (PCB) table, and external file management.
It simulates the behavior of the fork() and exec() system calls and logs all key operations.

## References

- *Silberschatz, Galvin, and Gagne*, Operating System Concepts, 10th Edition
- Linux Programmer’s Manual
- Course materials 
