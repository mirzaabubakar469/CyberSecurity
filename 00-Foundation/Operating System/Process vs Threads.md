## Process vs Threads

### Process

* Each process has its **own memory space**
* Processes are **independent**
* Communication between processes is **slower**
* Creating a process is **heavy and takes more resources**

### Thread

#### Key Points of Thread

* Threads share the **same memory**
* Threads are **lightweight**
* Communication between threads is **faster**
* Multiple threads improve **performance**

## User-Level Threads vs Kernel-Level Threads

### User-Level Threads (ULT)

**User-Level Threads** are managed by the **user-level thread library**, not by the operating system kernel.

#### Key Characteristics

* Managed in **user space**
* **Kernel is unaware** of these threads
* Thread management is done by **thread libraries**
* **Fast to create and manage**
* If one thread blocks, the **entire process blocks**

### Kernel-Level Threads (KLT)

**Kernel-Level Threads** are managed directly by the **operating system kernel**.

#### Key Characteristics

* Managed by the **operating system**
* Kernel **handles scheduling**
* Each thread can run **independently**
* If one thread blocks, **other threads continue**
* **Slower creation** compared to user threads
* **Higher overhead** because kernel is involved
