Testing disk performance with Linux

The easiest way is to use the Linux utility dd which is part of coreutils package :

* [Performance testing using dd](https://www.thomas-krenn.com/en/wiki/Linux_I/O_Performance_Tests_using_dd)

Note that dd can only test sequential read and write performance.

But there are also more sophisticated tools:

* [Flexible I/O tester](https://www.thomas-krenn.com/en/wiki/Fio_version_information)
* [Iozone](https://linux.die.net/man/1/iozone)
* [bonnie++ - program to test hard drive performance](https://linux.die.net/man/8/bonnie++)

