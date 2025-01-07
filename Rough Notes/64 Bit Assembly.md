## Register
- 64 bits 

# Quadword Pointer (QW)
- A **QWORD** (Quad Word) is a term used to describe a **64-bit** data type or pointer

# Memory Operations
```
mov rdi, qwordptr [rsi]
```

The above code goes as follows
- Make **rsi inside rsi as a pointer**
- **Remove 8 bytes (64 bits) from memory and put it in rdi**

## Store

```
mov qwordptr[rsi], rdi 
```
- Put the value of rdi in qwordptr

# How to make OS do something (Syscall)
- We **put values in a register and the value(number) does the below**  
- **We Perform operations like exit, read, write using a table with values for each operation**
- for sys_exit (exiting program) put **60 in rax register (for amd64)** check the table at 
  https://blog.rchapman.org/posts/Linux_System_Call_Table_for_x86_64/ 
  ![[2025-01-02 17-46-54.mkv]]
  