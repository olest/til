Memory pages and page faults

A page is a unit of memory, a fixed-length continuous block as used by the OS. Modern processors can
have support for multiple page sizes.

A transfer of pages between main memory and an auxiliary store, such as a hard disk drive, is referred to as 
paging or swapping.

A page fault occurs when a process tries to access a memory page without the required preparations. There are valid page faults
that can be resolved by loading the page content, for instance from a hard disk. An invalid page fault is a segmentation fault,
for instance when a memory address is requested that is not part of the address space.

* [wikipedia](https://en.wikipedia.org/wiki/Page_(computer_memory))
* [Memory Management Reference](https://www.memorymanagement.org/)
* Systems Performance : Enterprise and the cloud (Brendan Gregg)


