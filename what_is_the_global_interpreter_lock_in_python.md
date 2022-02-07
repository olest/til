What is the Global Interpreter Lock in python ?

Very good summary is [here](https://realpython.com/python-gil/).

Take home messages:
* Python bytecode is protected using mutex, is effectively running
single-threaded. 
* Any execution of bytecode needs acquire the lock
* Why is this done? Prevent race conditions in reference counting, easy to implement: only one global lock is needed
* Problem for CPU bound threads but I/O bound threads can still benefit (Example: web server)
* There are some proposals to remove the interpreter lock: [infoworld](https://www.infoworld.com/article/3637073/python-stands-to-lose-its-gil-and-gain-a-lot-of-speed.html)



