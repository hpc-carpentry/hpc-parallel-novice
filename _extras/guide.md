---
layout: page
title: "Instructor Notes"
---

# Instructor's Briefing

This document tries to describe what preparations are required of instructors
to make the workshop work as smooth as possible. In order to build the
materials for the workshop at your site, consult the `_config.yaml` file before
you generate the site with `make site`. It contains the 'environment variables'
that are specific to your workshop, such as the name of the login node, the
root folder of the shared file system etc.

## Rational

The lineup of lessons is meant to be as flexible as possible. Skip lessons if
needed.

### Recap: Changing the Environment

We start with environment variables as a recap and to get all learners on
board. Feel free to skip this if you know from the pre-workshop survey that
your learners are capable of this.

### Estimation of Pi for Pedestrians

This lessons introduces the computational working hours for all of this
material. We use this way to calculate pi as it is compute intensive and
typically doesn't need any I/O. As it is compute intensive it renders itself as
a good example to illustrate data parallelism. Other types of parallelism (task
parallelism, latency hiding, ...) are excluded from the material on purpose in
order to keep the cognitive load on the learners low.

In addition, this lesson does nothing more than profile the code to find hot
spots with respect to performance, i.e. runtime.

### Parallel Estimation of Pi for Pedestrians

This lesson uses `multiprocessing` to parallelise the code in a shared memory
environment.

### Higher levels of parallelism

This lesson introduces dask as a representative candidate for cloud-native
parallelisation approaches. This offers multiple things to the learners which
often induce trouble in understanding.

It shows that there are libraries out there that perform parallelization
automatically. It also tries to demo the infrastructure required for this, i.e.
setting up a server process that dispatches work to worker processes etc.

### Searching for Pi

This introduces concepts from high throughput computing by illustrating
map-reduce style searches through files.


Use the file
[generate_scrambled_data.py](./code/03_parallel_jobs/generate_scrambled_data.py)
to produce 16 files that comply to the files used in this section, e.g.:

```
pi_estimate_01.data  pi_estimate_07.data  pi_estimate_13.data
pi_estimate_02.data  pi_estimate_08.data  pi_estimate_14.data
pi_estimate_03.data  pi_estimate_09.data  pi_estimate_15.data
pi_estimate_04.data  pi_estimate_10.data  pi_estimate_16.data
pi_estimate_05.data  pi_estimate_11.data
pi_estimate_06.data  pi_estimate_12.data
```
{: .output}

This could be done like so:

~~~
for i in `seq -f "%02.0f" 1 16`
do
    python3 ./generate_scrambled_data.py pi_estimate_${i}.data
done
~~~
{: .language-bash}

At best, create directories for the each learner so that they don't get into
each other's way.

Note, that this lesson is currently quite fragile as the i/o caching can easily
get into the way of the learners.


### Bonus session: Distributing computations among computers

A guided tour through a MPI program with all it's nuances and brain quirks in
program flow.

