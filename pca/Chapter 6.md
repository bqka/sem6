# Linear Pipeline Processors

A linear pipeline processor is a cascade of processing stages which are linearly connected to perform a fixed function over a stream of data flowing from one end to the other. 

## Async and Sync Models

#### Asynchronous Model

![[Pasted image 20260308050925.png]]
![[Pasted image 20260308050958.png]]

#### Synchronous Model

![[Pasted image 20260308051019.png]]
![[Pasted image 20260308051208.png|500]]


![[Pasted image 20260308051052.png]]

## Clock and Timing Control

![[Pasted image 20260308051507.png]]

![[Pasted image 20260308051556.png]]

#### Clock Skewing

![[Pasted image 20260308051721.png]]

## Speedup, Efficiency and Throughput

total time to complete execution for k stage pipeline and n tasks
$$ T_k = [k + (n-1)]\tau$$
tau -> clock period
k -> time for first task
n-1 remaining task

for a non pipelined processor which has flow-through delay of $$k\tau$$
$$T_1 = nk\tau$$

#### Speedup Factor
![[Pasted image 20260308052216.png]]

yap about maximum speedup
![[Pasted image 20260308052347.png]]

![[Pasted image 20260308052430.png|400]]
#### Optimal Number of Stages
![[Pasted image 20260308052450.png]]

-> maximize a performance/cost ratio

![[Pasted image 20260308052657.png|500]]
![[Pasted image 20260308052714.png|500]]

#### Efficiency and Throughput

![[Pasted image 20260308052757.png]]

# Nonlinear Pipeline Processors

![[Pasted image 20260308053008.png]]

## Reservation and Latency Analysis
![[Pasted image 20260308053520.png]]
![[Pasted image 20260308053605.png]]
![[Pasted image 20260308053614.png|400]]

static pipeline -> single reservation table
dynamic pipeline -> more than one reservation table

no. of columns -> evaluation time of a given function
time for X = 8, Y = 6

#### Latency Analysis

![[Pasted image 20260308054200.png]]

no. of time units (clock cycles) between two initiations of a pipeline is called latency

basically if u shift the reservation table thingy to the right, there should be no collisions
shift by 1 unit = latency of 1 add

![[Pasted image 20260308054407.png]]

latency sequence -> sequence of permissible nonforbidden latencies bw task initiations

latency cycle -> latency sequence which repeats the same subsequence (cycle) indefinitely

![[Pasted image 20260308054717.png]]

avg latency = sum of all latencies / no. of latencies

ex. (1, 8)
avg = (1 + 8)/2 = 4.5

## Collision Free Scheduling

![[Pasted image 20260308060551.png]]

#### Collision Vectors

![[Pasted image 20260308060622.png]]

static pipeline -> p = 1 (ideal case) always achievable
(ya bro cuz js shift the diagonal one to the right and u good)

![[Pasted image 20260308060737.png]]

#### State Diagrams

![[Pasted image 20260308061311.png]]

basically, count the position of 0's, from the right and those are permissible latencies for a state, then to get next state, right shift by p (basically remove till that 0 is gone) and then bitwise OR with the initial collision vector

![[Pasted image 20260308061529.png|500]]
![[Pasted image 20260308061721.png]]

![[Pasted image 20260308062013.png]]
#### Greedy Cycles

MAL -> Minimum average latency

![[Pasted image 20260308062046.png]]

find simple cycles -> calculate average latency -> js take the minimum

## Pipeline Schedule Optimization

![[Pasted image 20260308062323.png]]
#### Delay Insertion

![[Pasted image 20260308062516.png]]

![[Pasted image 20260308062931.png]]

![[Pasted image 20260308062948.png]]

#### Pipeline Throughput

![[Pasted image 20260308063022.png]]

#### Pipeline Efficiency

![[Pasted image 20260308063212.png]]

![[Pasted image 20260308063146.png|500]]
![[Pasted image 20260308063250.png|500]]


