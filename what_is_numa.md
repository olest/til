What is NUMA ?

NUMA stands for Non-Uniform Memory Access. It is a computer architecture in which memory
is physically attached to a single or a group of the processors. 

This has significant implications for performance: the access latency for memory that is
further away from a CPU will be higher. If the operating system is aware of the cpu and
memory topology, it can schedule threads accordingly.

The numactl command can be used to bind processes to NUMA nodes. The numastat command
provides useful summary statistics such as memory allocations on the intended NUMA node etc.


* [wikipedia](https://en.wikipedia.org/wiki/Non-uniform_memory_access)
* [linuxhint.com](https://linuxhint.com/understanding_numa_architecture/)


