---
layout: lesson
root: .
---

"High-performance computing" supercomputers have been around for longer than some of their users today. The first supercomputer, the [Cray-1](https://en.wikipedia.org/wiki/Cray-1), was setup in 1976 and was put in operation at Los Alamos National Laboratory. In the course of history, the design of supercomputers underwent several revolutions. Today, most universities and an increasing part of the industry in several domains exploit the computational power of clusters of interconnected servers.

These High-performance Computing (HPC) clusters are used for large scale data processing and data analysis, scalable but yet fine grained parallel calculations and compute intensive simulations of ever increasing fidelity. This course material is meant to introduce learners to the core principles how to program applications that can harness the full power of such machinery. 

Please note that this lesson uses Python 3 without the intent of claiming python to be the universal language for HPC. Python is merely used as a vehicle to convey concepts that due to the intuitiveness of the language should be easy to transport to other languages and domains.

> ## Prerequisites
>
> This material targets future or present users of a HPC infrastructure of any discipline. The learners are expected to have programming skills beyond basic courses. Learners are expected to know how to submit a batch job on a HPC cluster. Further, knowledge on how to write functions and declare variables in python are required. Basic `numpy` array commands are beneficial but not required to follow the course.
> 
> In other words, learners are expected to have skills which are equivalent to having completed:
> 
> - [swcarpentry/shell-novice](https://swcarpentry.github.io/shell-novice/)
> - [swcarpentry/python-novice-inflammation](https://swcarpentry.github.io/python-novice-inflammation/)
> - [hpccarpentry/hpc-intro](https://carpentries-incubator.github.io/hpc-intro/) or [hpc-in-a-day's](https://psteinb.github.io/hpc-parallel-novice/) first 4 lessons
>
> This lesson guides you through the basics of parallelisation on a computer cluster (or batch farm or supercomputer). If you're already comfortable with using systems like LSF, Slurm or PBS/Pro and have written parallel applications to run on a cluster, you probably won't learn much from this lesson. But you are welcome to help others as a technical assistant or contribute to this [course material](https://psteinb.github.io/hpc-parallel-novice).
{: .prereq}
