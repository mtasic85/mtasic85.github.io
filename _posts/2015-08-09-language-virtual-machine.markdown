---
layout: post
title:  "Language Virtual Machine"
date:   2015-08-09 12:47:00
categories: vm
---

I will start here series about language virtual machines. I will first show native examples in C and in few other dynamic languages such as Python, Ruby and Lua. Their speeds will be compared.

After we have insight into what kind of speeds we expect from which programming language implementation, we will try to explore approaches in VM design and implementation.

Our main goal is to show speed of the simplest but functional possible VM's and some basic optimizations.

VM's will be written in C, C99 and in some cases C11 standard.

System (my home desktop computer) on which benchmarks will be run is following:

{% highlight bash %}

$ lscpu 
Architecture:          x86_64
CPU op-mode(s):        32-bit, 64-bit
Byte Order:            Little Endian
CPU(s):                4
On-line CPU(s) list:   0-3
Thread(s) per core:    1
Core(s) per socket:    4
Socket(s):             1
NUMA node(s):          1
Vendor ID:             AuthenticAMD
CPU family:            18
Model:                 1
Model name:            AMD A8-3850 APU with Radeon(tm) HD Graphics
Stepping:              0
CPU MHz:               2900.000
CPU max MHz:           2900.0000
CPU min MHz:           800.0000
BogoMIPS:              5792.15
Virtualization:        AMD-V
L1d cache:             64K
L1i cache:             64K
L2 cache:              1024K
NUMA node0 CPU(s):     0-3

$ uname -nsrm
Linux arch 4.1.4-1-ARCH x86_64

$ cat /proc/meminfo | grep MemTotal
MemTotal:        8170204 kB

{% endhighlight %}