**Concurrency** is the ability to execute multiple tasks by *alternating* the work of a number of given programs. This is done fast to give the *illusion* of a computer of being worked on simultaneously.

This can be done with a single or multiple CPU cores.

Meanwhile, this is not the same of **true** parallelism - that requires at least **two** or more CPU cores. 

**Parallelism** is the ability for hardware to truly execute two or more tasks simultaneously by leveraging existing computer hardware.

The resources to call a singular running piece of program code are [[Threads]]. Threads that share memory space and other resources are called **processes**.

Check [[Threads]] for more detailed information about how running code works.

# Significance
Imagine you are a computer science student in the *far ancient history of 1960s*.

You would have a computer program you want to run, but so do multiple people too. Many people want to use a computer, so you would have to line up and take turns. But it takes a *long* time for yours to get done. 

You noticed something in the line:
- Some programs you saw are just quick bursts, only taking a millisecond to run.
- Some take *hooouurrssss* to complete.
- Some programs you saw might have while loops that will never. stop. running. until the user is satisfied with it.

Knowing that computers have limited CPU cores and time to execute tasks. What would you want to do? Clearly some *schedule justice* needs to be done.


