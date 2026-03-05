![[Pasted image 20260302033853.png|500]]

![[Pasted image 20260302033938.png]]

the latter includes pipelined instruction execution, pipelined arithmetic computations, and memory-access operations. Pipelining has proven especially attractive in performing identical operations repeatedly over vector data strings. Vector operations were originally carried out implicitly by software-controlled looping using scalar pipeline processors.

#### Flynn's Classification

![[Pasted image 20260304035647.png]]

SISD -> conventional sequential machines
SIMD -> vector computers
MIMD -> parallel computers
MISD -> systolic arrays (for pipelined execution of specific algorithms)

#### Parallel/Vector Computers

![[Pasted image 20260304040228.png]]

![[Pasted image 20260304040410.png]]

```
Memory-to-Memory
Memory → Pipeline → Memory

Register-to-Register
Memory → Vector Registers → Pipeline → Vector Registers → Memory
```

pipelining -> temporal parallelism 
![[Pasted image 20260304040615.png|400]]
SIMD -> spatial parallelism

![[Pasted image 20260304040549.png]]

#### Development Layers

![[Pasted image 20260304040825.png]]

![[Pasted image 20260304041130.png]]

### System Attributes to Performance

**Clock Rate and CPI**
![[Pasted image 20260304042721.png]]

##### Performance Factors

![[Pasted image 20260304042743.png]]

![[Pasted image 20260304042831.png]]

$$f = 1/\tau$$
$$T = I_c \times CPI \times \tau$$
$$T = I_c \times (p + m \times k) \times \tau$$

##### System Attributes
![[Pasted image 20260304043200.png]]
![[Pasted image 20260304043224.png]]

**MIPS Rate**
![[Pasted image 20260304043213.png]]

**Throughput Rate**
![[Pasted image 20260304043430.png]]

### Programming Environments

![[Pasted image 20260306001724.png]]
![[Pasted image 20260306001740.png|500]]

**Implicit Parallelism**
![[Pasted image 20260306002003.png]]

**Explicit Parallelism**
![[Pasted image 20260306002027.png]]

# Multiprocessors and Multicomputers

## Shared Memory Multiprocessors

### UMA (Uniform Memory Access)
![[Pasted image 20260306002245.png|500]]
![[Pasted image 20260306002623.png]]

### NUMA (Non Uniform Memory Access)
![[Pasted image 20260306002651.png]]
![[Pasted image 20260306003243.png]]

### COMA (Cache Only Memory Access)
![[Pasted image 20260306003433.png]]
![[Pasted image 20260306003531.png]]

## Distributed Memory Multicomputers

![[Pasted image 20260306003759.png|500]]
![[Pasted image 20260306003922.png]]
Internode communication is carried out by passing messages through the static connection network.

# Multivector and SIMD Computers

## Vector Supercomputers
![[Pasted image 20260306005302.png|500]]
![[Pasted image 20260306005326.png]]
![[Pasted image 20260306005747.png]]

### SIMD Supercomputers
![[Pasted image 20260306005944.png|500]]

![[Pasted image 20260306010041.png]]

# PRAM Model

## Parallel Random Access Machines
![[Pasted image 20260306011033.png]]
![[Pasted image 20260306011143.png]]
![[Pasted image 20260306011150.png]]
![[Pasted image 20260306011454.png]]

