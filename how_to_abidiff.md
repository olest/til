
Jason Turner dedicated a recent episode of C++ weekly to [abidiff](https://man7.org/linux/man-pages/man1/abidiff.1.html).
abidiff is a tool to check for changes in the Application Binary Interfaces 
[ABI](https://en.wikipedia.org/wiki/Application_binary_interface) in shared libraries. Abidiff is part of 
[libabigail](https://developers.redhat.com/blog/2014/10/23/comparing-abis-for-compatibility-with-libabigail-part-1).

But what is an [ABI change](https://www.youtube.com/watch?v=By7b19YIv8Q)?

The ABI is a broad concept: it comprises the processor instructions used in the library, it defines the mechanics of
function calls and the layout of the library file and how to navigate it.

The man page of abidiff recommends to compile with -g to get legible symbol names. Jason Turner shows another alternative,
using c++filt.

