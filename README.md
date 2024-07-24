# Computer Organization Developing the L1 Cache for the μRISC-V Processor

![cache1_1](https://github.com/user-attachments/assets/697c80ee-962e-4456-a51e-758db76db9ea)


## Introduction
I have to develop cache replacement policies, and these policies should be

implemented in the open-source RISC-V emulator, Spike. By implementing the policies with the cache simulation interfaces exposed by Spike,the RISC-V processor emulator can further estimate the performance delivered by various cache models. Note that the original version of Spike has implemented the mechanism of cache simulations. That is, users can enable the cache simulations by specifying which types of the cache simulations to be performed via parameter settings. Unfortunately, the current version of Spike only implements the random replacement policy and some other policies should be implemented in order to better evaluate different design alternatives.

Specifically, you are required to implement the three replacement policies.


## Three Cache Replacement Policies

As a cache replacement policy can greatly affect the cache hit/miss rate, it has been extensively studied and hence, many replacement polices have been proposed, each suitable for some purposes. The cache hit/miss rate is an important metric to evaluate the efficiency of a cache design. In this assignment, your designs are evaluated solely by the miss rate. You are required to implement the following three policies and to report their miss rates to get some scores of this assignment.
The three of the most commonly seen cache replacement policies are listed below. These three policies are served as the baseline policies to be implemented in this assignment.
### 1. First In First Out (FIFO): The cache behaves the same as a FIFO queue, where it evicts the cache blocks in the same order as they were added to the cache without considering any other factors.
### 2. Least Recently Used (LRU): Those the least recently used cache blocks are discarded first.
### 3. Least-Frequently Used (LFU): Those cache blocks that are used least often are replaced first.



