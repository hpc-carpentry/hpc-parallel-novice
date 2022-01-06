---
title: "Profiling parallel programs"
teaching: 45
exercises: 10
questions:
- "How do I profile a program using the message passing interface (MPI)?"
objectives:
- "Profile a program to examine computation and communication bottlenecks"
keypoints:
- "Profiling can help explain how to speed up code."
- "Parallel profiling tools are similar to serial ones, but typicaly add
   communication and computation imbalance information"
---

## Parallel Profiling and Tracing Tools

There are a number of portable open source parallel profiling and tracing tools
including
- [HPCToolkit](http://hpctoolkit.org/)
- [Extrae](https://tools.bsc.es/extrae)
- [Scalasca](http://www.scalasca.org/)
- [TAU](https://www.cs.uoregon.edu/research/tau/home.php)
