# XV Quiz (CSL 3030)

Welcome to the XV Quiz for CSL 3030 - Operating Systems!



## Instructions
- Answer the multiple-choice questions by selecting the correct option.
- For theoretical questions, provide concise and accurate explanations.
- Feel free to use this quiz for self-assessment or educational purposes.

## Multiple-Choice Questions

#### Question 1: Basics
1. What is XV6?
   - a. A programming language
   - b. A Unix-like operating system
   - c. A file system
   - d. An assembly language

#### Question 2: Architecture
2. XV6 is based on which earlier operating system?
   - a. Windows
   - b. Linux
   - c. BSD
   - d. DOS

#### Question 3: File System
3. Which file system is used in XV6?
   - a. FAT32
   - b. NTFS
   - c. ext4
   - d. simple

#### Question 4: System Calls
4. How are system calls implemented in XV6?
   - a. As functions in the C standard library
   - b. As interrupts
   - c. Through the command line
   - d. As external programs

#### Question 5: Processes
5. In XV6, what is the maximum number of processes that can run simultaneously?
   - a. 128
   - b. 256
   - c. 512
   - d. 1024

#### Question 6: Shell
6. What is the name of the shell used in XV6?
   - a. Bash
   - b. Zsh
   - c. Sh
   - d. Fish

#### Question 7: Scheduling
7. How does XV6 handle process scheduling?
   - a. Round-robin scheduling
   - b. Priority-based scheduling
   - c. First-Come-First-Serve (FCFS)
   - d. Random scheduling

#### Question 8: Memory Management
8. Which memory management technique is used in XV6?
   - a. Paging
   - b. Segmentation
   - c. Virtual Memory
   - d. None of the above

#### Question 9: Interrupts
9. How are interrupts handled in XV6?
   - a. Through polling
   - b. Using hardware interrupts
   - c. Using software interrupts
   - d. Both b and c

#### Question 10: Multithreading
10. Does XV6 support multithreading?
    - a. Yes
    - b. No

#### Bonus Question:
11. Who developed XV6?
    - a. Microsoft
    - b. Google
    - c. MIT
    - d. IBM

## Theoretical Questions

#### Question 12: Process States
12. Briefly explain the different states a process can be in within the XV6 operating system.

#### Question 13: File System Structure
13. Describe the structure of the file system in XV6. Include the key components and their roles.

#### Question 14: System Calls vs. Library Functions
14. Explain the difference between system calls and library functions in the context of XV6. Provide examples of each.

#### Question 15: Memory Paging
15. How does memory paging work in XV6? Discuss the benefits of using paging in memory management.

#### Question 16: Shell Commands
16. Name and briefly explain three essential shell commands in the XV6 operating system.

#### Question 17: Process Synchronization
17. Discuss the concept of process synchronization in XV6. Why is it essential, and what mechanisms are used to achieve it?

#### Question 18: Interrupt Handling
18. Explain the role of interrupts in the XV6 operating system. How are interrupts handled, and what is their significance in system operation?

#### Question 19: Virtual Memory
19. What is virtual memory, and how is it implemented in XV6? Discuss the advantages of using virtual memory.

#### Question 20: Boot Process
20. Outline the steps involved in the boot process of XV6. What happens from the moment the computer is powered on to when the XV6 kernel is loaded into memory?

## Answers
1. b. A Unix-like operating system
2. b. Linux
3. d. simple
4. a. As functions in the C standard library
5. a. 128
6. c. Sh
7. a. Round-robin scheduling
8. a. Paging
9. d. Both b and c
10. b. No
11. c. MIT
12. Answer
   1. Unused: process before the allocation of resources any resources
   2. Embryo: when new process is created and is not allocated a stack and a page table
   3. Sleeping: when sleep() syscall is used
   4. Runnable: When the process is ready to be executed but not currently in the CPU
   5. Running: When the process is getting executed in the CPU
   6. Zombie: When a process has finished executing but the resources that were used by it are not freed
13. Answer
    The XV6 file system is orgaised in 7 layers in an heirarchial structure, the layers are:
    File Descriptor: file descriptor layer abstracts many Unix resources (e.g., pipes, devices, files, etc.) using the file system interface
    Pathname: The pathname layer provides hierarchical path names like /bin/ys/xys/xyz, and resolves them with recursive lookup
    Directory: A directory can contain a group of files or other directories
    Inode:  The inode layer provides individual files, each with a unique i-number
    Logging: The logging layer allows higher layers to wrap updates to several blocks in a transaction, and ensures that the blocks are updated atomically in the face of crashes
    Buffer Cache: The Buffer Cache layer caches disk blocks and synchronizes access to them, making sure that only one kernel process at a time can modify the data stored in any particular block.
    Disk: Disk hardware traditionally presents the data on the disk as a numbered sequence of 512-byte blocks
14. 

15. System calls in XV6 are implemented in the kernel mode library functions are executed in user mode.
    
     
