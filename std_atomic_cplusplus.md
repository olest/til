What is std::atomic? See [here](https://en.cppreference.com/w/cpp/atomic/atomic).

> Each instantiation and full specialization of the std::atomic template defines an atomic type. If one 
> thread writes to an atomic object while another thread reads from it, the behavior is well-defined. 

What is it good for?

An atomic type enables atomic operations. These operations are indivisible, they cannot be observed 
half-done from any thread. 

The main use-case for atomic operations as a replacement for operations that would otherwise use a mutex.

Related links:

[stackoverflow: what exactly is stdatomic?](https://stackoverflow.com/questions/31978324/what-exactly-is-stdatomic)

[Using atomics for thread synchronization in C++](https://www.justsoftwaresolutions.co.uk/2021/04/)

[C++ memory models](https://preshing.com/20120930/weak-vs-strong-memory-models/)

