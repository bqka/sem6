![[Pasted image 20260307010830.png|367]]
![[Pasted image 20260307011244.png|544]]
![[Pasted image 20260307011316.png|378]]
![[Pasted image 20260307011437.png|418]]

Processors and Coprocessors The central processor of a computer is called thecentral processing unit (CPU) as illustrated in Fig. 4.3. This CPU is essentially a scalar processor, which may consist of multiple functional units such as an integer arithmetic and logic unit (ALU), a floating-point accelerator, etc. The floating-point unit can be built on a coprocessor (Fig. 4.3b) which is attachedto the CPU. The coprocessor executes instructions dispatched from the CPU. A co- processor may be a floating-point accelerator executing scalar data, vector processor executing vector operands, a digital signal processor (DSP), or a Lisp processor execut- ing AI programs. Coprocessors cannot handle I/O operations.

![[Pasted image 20260307011920.png|595]]

![[Pasted image 20260307012001.png|610]]

![[Pasted image 20260307012417.png|463]]


![[Pasted image 20260307022054.png|545]]
![[Pasted image 20260307022115.png|558]]
![[Pasted image 20260307022129.png|567]]
![[Pasted image 20260307022442.png|590]]
![[Pasted image 20260307022601.png|563]]


![[Pasted image 20260307022306.png|574]]
![[Pasted image 20260307022315.png|577]]
![[Pasted image 20260307022803.png|453]]

![[Pasted image 20260307022948.png]]
![[Pasted image 20260307023343.png]]

 vector processor can assume either a register-to-register architecture or a memory- to-memory architecture. The former uses shorter instructions and vector register files. The latter uses memory-based instructions which are longer in length, including memory addresses.

![[Pasted image 20260307023656.png|501]]

Vector Pipelines
![[Pasted image 20260307023719.png|466]]

![[Pasted image 20260307023801.png|509]]

![[Pasted image 20260307023828.png|509]]![[Pasted image 20260307023837.png|300]]
![[Pasted image 20260307023847.png|497]]


### Memory Hierarchy 

![[Pasted image 20260307024050.png|461]]
![[Pasted image 20260307024208.png|496]]


#### 1. Basic Idea

The book explains that **no single memory technology can simultaneously provide**:

- very **high speed**
- very **large capacity**
- very **low cost**

Fast memories are expensive and small, while large memories are slower but cheaper.  
Therefore computer systems organize memory into a **hierarchy of storage levels**, where each level differs in **speed, size, and cost**.

This structure is called **memory hierarchy technology**.

#### 2. Structure of the Memory Hierarchy

The hierarchy is typically organized from **fastest and smallest to slowest and largest**.
##### Typical hierarchy

1. **CPU Registers**
2. **Cache Memory**
3. **Main Memory (RAM)**
4. **Secondary Storage (Disk / SSD)**
5. **Archival Storage (tapes, etc.)**

#### 3. Characteristics of Each Level

##### 1. CPU Registers

- Located **inside the processor**
- **Fastest memory**
- Very **small capacity**
- Used to store **immediate operands and intermediate results**

Access time: **1 CPU cycle**

##### 2. Cache Memory

Cache is a **small high-speed memory located between CPU and main memory**.
Purpose:
- Reduce the time needed to access frequently used data.

Features:
- Very fast
- Smaller than main memory
- Stores **copies of frequently accessed instructions and data**

The book describes cache as a way to **bridge the speed gap between processor and main memory**.

##### 3. Main Memory

Main memory (RAM) stores:
- active programs
- data currently used by the processor

Characteristics:
- Larger capacity than cache
- Slower than cache
- Directly accessible by CPU

##### 4. Secondary Storage

Examples:
- Hard disks
- Solid state drives

Characteristics:
- Very **large capacity**
- **Much slower** than main memory
- Used for **permanent storage**
##### 5. Archival Storage

Examples:
- Magnetic tapes
- Optical storage

Used for:
- Backup
- Long-term data storage

Access time is **very slow**, but storage capacity is very large.

#### Goals of Memory Hierarchy Technology

The  memory hierarchy aims to:

1. **Reduce memory access time**
2. **Increase overall system performance**
3. **Provide large storage capacity**
4. **Maintain reasonable system cost**

Thus the hierarchy provides the **illusion of a large, fast, and inexpensive memory system**.



![[Pasted image 20260307030518.png|528]]
![[Pasted image 20260307030539.png|532]]
![[Pasted image 20260307030555.png|483]]
![[Pasted image 20260307030607.png|478]]
![[Pasted image 20260307030739.png|490]]



![[Pasted image 20260307031221.png|588]]
![[Pasted image 20260307031243.png|588]]

![[Pasted image 20260307031257.png|584]]

![[Pasted image 20260307031310.png|608]]
![[Pasted image 20260307031323.png|607]]

![[Pasted image 20260307031336.png|610]]

