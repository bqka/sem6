# Performance Metrics and Measures

![[Pasted image 20260307005943.png]]
## Parallelism Profile in Programs

![[Pasted image 20260307005749.png]]
![[Pasted image 20260307010148.png]]

#### Average Parallelism

Assumptions
![[Pasted image 20260307010425.png]]
![[Pasted image 20260307010445.png]]

total work done
![[Pasted image 20260307010540.png|400]]
![[Pasted image 20260307010608.png|400]]
![[Pasted image 20260307010621.png|400]]
![[Pasted image 20260307010708.png]]

#### Available Parallelism
![[Pasted image 20260307011616.png]]
![[Pasted image 20260307011634.png]]

#### Asymptotic Speedup

![[Pasted image 20260307011917.png]]

ti(inf) = Wi / i (delta)
because max dop is i, so if infinite processors, each portion runs parallely on i processors
$$S_{\infty} = \text{Average Parallelism}$$

![[Pasted image 20260307012329.png]]

Maximum Speedup=Average Parallelism
because speedup depends on **how much parallel work is done over time**, not just the peak parallel capability.

## Harmonic Mean Performance

#### Arithmetic Mean Performance

![[Pasted image 20260307012556.png]]
![[Pasted image 20260307012710.png|500]]
#### Geometric Mean Performance

![[Pasted image 20260307012635.png]]
![[Pasted image 20260307012724.png|500]]

![[Pasted image 20260307012926.png]]

Execution Rate = 1/Execution Time

#### Harmonic Mean Performance

![[Pasted image 20260307013059.png]]

#### Harmonic Mean Speedup

Harmonic mean speedup is used to compute the effective speedup of a program that executes using different numbers of processors for different fractions of time.

![[Pasted image 20260307013444.png]]

![[Pasted image 20260307013520.png|600]]
![[Pasted image 20260307013531.png|600]]
![[Pasted image 20260307013637.png]]

## Efficiency, Utilization and Quality

![[Pasted image 20260307015125.png|600]]
![[Pasted image 20260307015336.png|600]]
![[Pasted image 20260307015400.png|600]]
![[Pasted image 20260307015442.png|500]]

understanding

![[Pasted image 20260307015924.png|500]]
![[Pasted image 20260307015952.png|500]]

also, o(1) = t(1)

# Characteristics of Parallel Algorithms

### 1. Deterministic vs Non-deterministic
- **Deterministic algorithms** always produce the **same output for the same input**.
- Only deterministic algorithms are **practically implementable on real machines**.
- Studies usually focus on **deterministic algorithms with polynomial time complexity**.
### 2. Computational Granularity
Granularity determines the **size of computation tasks**.
Types:
- **Fine-grain** → small tasks, frequent communication
- **Medium-grain** → moderate task size
- **Coarse-grain** → large tasks, less communication

Granularity affects **performance and communication overhead**.
### 3. Parallelism Profile
Parallelism profile describes the **distribution of parallel work during execution**.
It shows:
- how much parallelism exists
- when processors can work simultaneously

This directly affects **efficiency of parallel execution**.
### 4. Communication Patterns & Synchronization
Parallel algorithms require **communication between processors**.
Types:
- **Static communication** → fixed pattern
- **Dynamic communication** → changes during execution

Notes:
- Static patterns suit **SIMD or pipeline machines**
- Dynamic patterns suit **MIMD machines**
- Frequent synchronization may **reduce efficiency**.
### 5. Uniformity of Operations
This refers to whether **the same type of operations are applied to all data**.

- Uniform operations → good for **SIMD and pipelining**
- Random or varied operations → better suited for **MIMD systems**
### 6. Memory Requirement & Data Structures

Large parallel problems require **large memory space**.
Performance depends on:
- **data structures used**
- **data movement patterns**
- **memory efficiency**
Both **time complexity and space complexity** influence the **granularity of a parallel algorithm**.

# Speedup Performance Laws

## Amdahl's Law for a Fixed Workload

In many real applications, the **problem size is fixed**.
When more processors are added:
- The same workload is **distributed among more processors**.
- The goal is to **reduce execution time**.
The resulting speedup is called **fixed-load speedup**.

![[Pasted image 20260307021432.png|400]]
![[Pasted image 20260307021827.png|400]]

![[Pasted image 20260307021904.png|500]]

![[Pasted image 20260307021922.png]]

![[Pasted image 20260307021938.png|500]]
![[Pasted image 20260307022002.png|500]]
![[Pasted image 20260307022058.png|400]]

#### Amdahl's Law Revisited

![[Pasted image 20260307022414.png|500]]
![[Pasted image 20260307022435.png|500]]
![[Pasted image 20260307022444.png|500]]

![[Pasted image 20260307022523.png]]

#### Sequential Bottleneck

if n -> infinity,
$$S_n = 1/\alpha$$
So speedup is **limited by the sequential fraction**.

## Gustafson's Law for Scaled Problems

![[Pasted image 20260307024129.png|600]]

![[Pasted image 20260307024159.png|600]]

![[Pasted image 20260307024341.png]]

![[Pasted image 20260307024405.png|600]]
![[Pasted image 20260307024456.png|600]]

understanding
![[Pasted image 20260307024617.png|600]]
![[Pasted image 20260307024753.png|500]]

#### Gustafson's Law

![[Pasted image 20260307024857.png|600]]
![[Pasted image 20260307025005.png]]
## Memory Bounded Speedup Model

![[Pasted image 20260307025319.png|500]]
![[Pasted image 20260307025354.png]]

![[Pasted image 20260307025402.png|600]]

![[Pasted image 20260307025451.png|500]]
![[Pasted image 20260307025509.png]]
![[Pasted image 20260307025516.png]]

#### Fixed Memory Speedup

![[Pasted image 20260307025544.png|600]]
![[Pasted image 20260307025555.png|500]]

![[Pasted image 20260307030104.png]]
![[Pasted image 20260307030001.png]]
![[Pasted image 20260307030009.png]]

![[Pasted image 20260307030233.png]]

