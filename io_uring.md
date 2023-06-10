## io_uring

io_uring is an asynchronous interface to the Linux kernel. It provides a mechanism to batch syscall which are expensive.

It can result in performance gains for file and network I/O, since fewer syscalls mean less context switching.  

The io_uring interface has 2 ring buffers,

* Submission queue (SQ): for submitting an I/O operation.
* Completion queue (CQ): for the result (data and status) of that I/O operation.

These ring buffers acts as queues between user space and kernel.


### References

* [io_uring manpage](https://manpages.debian.org/unstable/liburing-dev/io_uring_setup.2.en.html)
* [io_uring explained](https://unzip.dev/0x013-io_uring/)
* [Why you should use io_uring for network I/O](https://developers.redhat.com/articles/2023/04/12/why-you-should-use-iouring-network-io)
* [ io_uring is not an event system](https://despairlabs.com/blog/posts/2021-06-16-io-uring-is-not-an-event-system)
* [How io_uring and eBPF Will Revolutionize Programming in Linux](https://thenewstack.io/how-io_uring-and-ebpf-will-revolutionize-programming-in-linux)


