# Abstractions of Operating System

processes, virtual memory, files and virtual machine

------

## Processes: abstractions for the processor, main memory, and I/O devices.

A process is the operating system's abstraction for a running program.

Multiple processes can run concurrently (mean that the instructions of one process are interleaved with the instructions of another process) on the same system.

The operating system performs this interleaving with a mechanism known as context switching so that multicore processors can execute several programs simultaneously.

- Context: the state information (such as the current values of the PC, the register file, and the contents of main memory) that the process needs in order to run.
- Context switch: saving the context of the current process, restoring the context of the new process, and then passing control to the new process. When it switch to an old process, it is called interrupt return.

Threads: execution units in a process, each thread is a single control flow of a process.

- Each running in the context of the process and sharing the same code and global data.
- Threads are more efficient than processes.

------

## Virtual memory: the abstraction for both the main memory and I/O devices

It provides each process with the illusion that it has exclusive use of the main memory. 

Each process has the same uniform view of memory, which is known as its virtual address space.

The virtual address space seen by each process consists of a number of well-defined areas, each with a specific purpose.

- Program code and data.
  - These areas are initialized directly from the contents of an executable object file.
  - The area fixed in size once the process begins running.
- Heap or run-time heap. 
  - Following the program code and data area immediately.
  - The heap expands and contracts dynamically at run time as a result of calls to C standard library routines.
- Shared libraries.
  - Such as C standard library and math library.
  - Near the middle of the address space.

- Stack or user stack.
  - The compiler uses it to implement function calls.
  - Expend and contract dynamically during  the execution of the program.
  - Call a function -> stack grows.
  - Return from a function -> stack contracts.
- Kernel virtual memory.
  - The kernel is the part of the operating system that is always resident in memory.
  - Applications are not allowed to read or write the contents of this area or to directly call functions defined in the kernel code.

------

## Files: abstractions for I/O devices.

A file is a sequence of bytes, nothing more and nothing less.

Unix I/O is a small set of system calls for reading(for input) and writing (for output) files.

It provides applications with a uniform view of all of the varied I/O devices.

------

## Virtual machine: 

virtual machine is an abstraction of the entire computer, including the operating system, the processor  and the programs.

Introduced by IBM in 1960s

A way to manage computers that must be able to run programs designed for multiple operating systems or different versions of the same operating system.

