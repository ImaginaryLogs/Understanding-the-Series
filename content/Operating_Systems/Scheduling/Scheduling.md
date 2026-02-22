CPU **scheduling** solve the decision of which process gets to use the CPU when multiple processes are ready to execute.

Some key goals:
- Maximize CPU **utilization** - up and running doing useful work.
- Minimize *waiting time and turnaround time*
- Ensure **fairness** among processes
- Maintain *system responsiveness*

CPU Scheduling Algorithms should be thought of with these in mind. 

# Key Metrics
To understand a CPU Algorithm, key metrics are used to understand it.
## Schedule Metrics
Metrics for each thread that are given in a problem for the scheduler to solve.
- **Arrival Time (AT)**: When a process enters the ready queue.
- **Burst Time (BT)**: CPU time required by a process.
- **Completion Time (CT)**: When a process finishes execution.
## Thread Metrics
Metrics for each thread to understand how effectiveness of the system.
- **Turnaround Time (TAT)**: total time from arrival to completion. 

$$\text{TAT} = \text{CT} - \text{AT}$$

- **Waiting Time (WT)**: time spent waiting in ready queue since start.
$$
\text{WT} = \text{TAT} - \text{BT}
$$
## System-wide metrics
Metrics of the entire system.
- **Average Waiting Time**: The sum of all WT / Number of processes.
$$
\frac{\sum_{i = 0}^{n} WT_i}{n} = \frac{WT_0 + WT_1 + \cdots + WT_n}{n}
$$
- **Average Turnaround Time**: The sum of all TAT / Number of processes.

$$
\frac{\sum_{i = 0}^{n} TAT_i}{n} = \frac{TAT_0 + TAT_1 + \cdots + TAT_n}{n}
$$

# Scheduling Algorithms
**Non-preemptive** - once a process starts executing, it runs to completion.

- [[First Come First Serve]] (FCFS)
- [[Shortest Job First]] (SJF)
- [[Non-Preemptive Priority Scheduling]] (NPPS)
- [[Preemptive Shortest Remaining Time First]] (PSRTF)
- [[Round Robin]] (RR)

# Comparisons

| Algorithm     | Preemptive? | Starvation Risk | Avg WT | Best For               | Worst Case                         |
| ------------- | ----------- | --------------- | ------ | ---------------------- | ---------------------------------- |
| FCFS          | No          | No              | High   | Simple batch           | Long process first (convoy effect) |
| SJF           | No          | Yes             | Low    | Batch with known times | Unknown burst times                |
| RR            | Yes         | No              | Medium | Time-sharing           | Wrong quantum selection            |
| Priority (NP) | No          | Yes             | Varies | Real-time systems      | Low priority processes             |
| SRTF          | Yes         | Yes             | Lowest | Known short jobs       | Long processes starve              |
