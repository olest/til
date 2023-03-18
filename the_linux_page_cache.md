The Linux Page cache explained 

Page cache is part of the Virtual File System, all reads and writes go through it. 

It uses a [write-back algorithm](https://en.wikipedia.org/wiki/Cache_%28computing%29#Writing_policies). The 
typical page size is 4K.

The Linux kernel will often read ahead and load more data into RAM than your program reads. The tool vmtouch can show diagnostics regarding the number memory pages cached per file.

Pages that are stored in the cache and then modified, are called dirty pages. It is expensive to flush dirty pages from the cache since they need to be written to disk.


* [The Linux Page Cache for SRE](https://biriukov.dev/docs/page-cache/0-linux-page-cache-for-sre/)
* [The Linux Page Cache for SRE - code examples](https://github.com/brk0v/sre-page-cache-article)


