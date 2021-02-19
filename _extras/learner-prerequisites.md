---
title: Learner Prerequisites
---

This page collects questions that learners can answer in order to judge if they 
bring all prequisites to the course.

# Required Pre-Knowledge

- **Basic Shell** – Navigating directories, Copy/Moving, writing shell scripts, 
using the environment, using wildcards

- **Basic Python** – Writing python scripts, writing python functions, array slicing


# Pre-Workshop Survey

For a motivation of this survey type, see [Greg Wilsons Template in Teaching 
Tech Together](https://teachtogether.tech/en/index.html#s:checklists-preassess).

## Shell

### Moving Things

You are provided with a directory of `300` files that end with `.log`, `.data` 
and `.err` at equal proportions. You like to rename all `.log` files to `.out` 
files. How do you do this?

1. I can do that. Give me a shell and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.

### Moving around

You are on `/bigdata/users/wolfman/projects/study` and want to jump over to 
`/bigdata/projects/experiments/at-moonlight` on the command line.

1. I can do that. Give me a shell and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.

### Collaborator Candy

A collaborator provides you an implementation of a state-of-the-art simulation 
that you need to compare your own predictions to. He tells you: "You can use it on the command line
right away. Unpack the file I sent you and use the `sim` executable in the 
`bin/` folder from it. The rest is explained in the output of the `--help` flag." 
You want to execute `sim` on your cluster. How do you set up your shell for this?

1. I can do that. Give me a shell and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.

### Automating All The Things

You observe yourself copy and pasting the same sequence of 5 commands on the command line for more 
than three times during a day. You alert yourself that you should write a script 
for this now. The script requires two input arguments, i.e. two single file locations, 
to perform it's duty.

1. I can do that. Give me a shell and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.

## Python

### Lists 1

You are provided with a python list of integer values. The list has length 1024 and you would like to obtain all entries from index 50 to 101. How would you do this? 

1. I can do that. Give me something that understands python and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.


### Lists 2

You are provided a list of 512 random float values. These values range between 0 and 100. You would like to remove any entry in this list that is larger than 90 or smaller than 10. 

1. I can do that. Give me something that understands python and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.

### Numpy

You are provided two `np.ndarray` objects with shape `(32,16)` each. The objects are called `x` and `y`. You would like to element-wise compute `x[i]*y[i] + 42`. How do you do that?

1. I can do that. Give me something that understands python and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.

### Modularization 1

You observe yourself copy-and-paste'ing 5 lines of your code over and over again. You decide the put these lines into a function. For this, the function requires 3 input parameters. The parameters are a file location, a specific object hash (i.e. a string) and a parameter that controls the verbosity of the function. The latter parameter has the default value "False".  

1. I can do that. Give me something that understands python and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.


## Parallelisation

### Common Choices

A compute task on your laptop takes 2 hours to complete. You fed 150 input files to a single application that was started on the command line. You mention this issue in the weekly group meeting. A team member mentions that similar issues were resolved in the past by using a powerful workstation of your room mate, a compute server of the institute located in the cellar, by using the university data center or by purchasing cloud server infrastructure. Which one do you choose most likely?

1. powerful workstation of your room mate
2. a compute server of the institute located in the cellar
3. the university data center
4. purchasing cloud server infrastructure

### Jobs, Jobs, Jobs

A compute task on your laptop takes more than 2 hours to complete - you kill the task and reconsider your approach. You feed 50 input files to a single application that needs to run once for every input file. You conclude that this is a good task for your cluster. You sit down and submit several jobs to the cluster. Each job is limited to 10 minutes of the walltime. Each job defines an output file of the structure `done_${FILENAME}.log` where `${FILENAME}` refers to the location of your input file. 

1. I can do that. Give me a shell on a cluster and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.

### Multi-Parallel on one machine

One of the goto tools of your domain has just been released on github with a version that can employ multiple cores on a single computer. You want to put this software to use on your cluster. For this, you submit a job that requires 32 cores on one machine and 64 GB of RAM if available. 

1. I can do that. Give me a shell on a cluster and I'll show you.
2. I'd need to look up the syntax in a cheatsheet or some old code and I'm good to do this.
3. I am unclear about this, I'd have to consult a colleague or a search engine to do this.
4. I am not sure what to do.
