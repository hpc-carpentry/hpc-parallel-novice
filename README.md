# Introduction to Parallelisation on HPC platforms

Novice introduction to parallelisation with high performance computing. This material was conceived as a sandbox project for [hpc-carpentry](https://hpc-carpentry.org). This work derives from [hpc-in-a-day](https://github.com/psteinb/hpc-in-a-day) but will not be kept in sync.

## Material

The material can be viewed [here](https://psteinb.github.io/hpc-parallel-novice)!

## Audience

The material targets future users of a HPC infrastructure of any discipline. The learners are expected to have an introductory level of programming skills. Learners are expected to know how to submit a batch job on a HPC cluster. Further, knowledge on how to write functions in python are required. Basic `numpy` array commands are beneficial but not required to follow the course.

## Scheduler

This material tries to be scheduler agnostic. Currently, it supports LSF and SLURM. The job scheduler type can be set with the `workshop_scheduler` variable in [_config.yaml](./_config.yaml).

# How to build

## Dependencies

The material is based on the [software carpentry lesson template](https://github.com/swcarpentry/styles). It hence depends on a fairly recent version of [jekyll](jekyllrb.org). Just give building it with `make site` in the root directory a try. If you find any problems, please open an issue.

## local tests

To test the material locally, open a terminal and type:

```
$ make serve
# ...
    Server address: http://127.0.0.1:4000
  Server running... press ctrl-c to stop.
```

Once you see the above, open a web browser on the same machine and copy \& paste `http://127.0.0.1:4000` in the URL address field. Load this page and you should see a local version of the material display. Exit the rendering as prompted by pressing `ctrl-c`.
