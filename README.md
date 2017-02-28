# unswapd
unswap processes during times of low system load and low memory usage

# motivation
a number of host monitoring systems use a very simplistic method of determining host memory related issues.  They may issue an alert when swap memory has hit 90 percent usage even if the main memory usage has returned to below threshold levels.

Ths implementation addresses the issue by returning those processes to the main memory.  Other methods, such as flushing VM caches or turning swap off and on again present additional issues of their own.
