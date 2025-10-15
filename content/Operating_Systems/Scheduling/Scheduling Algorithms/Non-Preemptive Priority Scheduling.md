Each process has a priority number. Process with highest priority executes first. 

Non-preemptive: once started, runs to completion.

### Example Problem 

**Rule**: Lower number = Higher priority

|Process|Arrival Time|Burst Time|Priority|
|---|---|---|---|
|P1|0|4|2|
|P2|1|3|1|
|P3|2|1|3|
|P4|3|2|2|

### Solution Steps

1. **At time 0**: Only P1 → P1 executes (0-4)
2. **At time 4**: P2, P3, P4 available. Highest priority is P2 (1) → P2 executes (4-7)
3. **At time 7**: P3, P4 available. P1 and P4 both have priority 2, but P4 arrived later, P3 has priority 3
    - P4 executes (7-9)
4. **At time 9**: P3 executes (9-10)

|Process|AT|BT|Priority|CT|TAT|WT|
|---|---|---|---|---|---|---|
|P1|0|4|2|4|4|0|
|P2|1|3|1|7|6|3|
|P3|2|1|3|10|8|7|
|P4|3|2|2|9|6|4|

**Average WT** = (0 + 3 + 7 + 4) / 4 = **3.5**  
**Average TAT** = (4 + 6 + 8 + 6) / 4 = **6**

### Advantages

- Important processes get CPU first
- Flexible (can assign priorities based on various criteria)
- Good for real-time systems
- Can differentiate between system and user processes

### Disadvantages

- **Indefinite blocking (Starvation)**: Low-priority processes may never execute
- Priority inversion problems
- Requires knowledge of priority assignment
- Can be unfair to lower-priority processes
- **Solution to starvation**: Aging (gradually increase priority of waiting processes)