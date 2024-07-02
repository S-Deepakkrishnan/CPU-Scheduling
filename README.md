This is a comprehensive description of CPU scheduling algorithms along with their functionalities and criteria. Here's a more detailed explanation of each algorithm:

### CPU Scheduling Algorithms

#### 1. **First Come First Serve (FCFS)**
- **Type:** Non-Preemptive
- **Criteria:** Processes are executed in the order they arrive in the ready queue.
- **Pros:** Simple to implement.
- **Cons:** Can lead to the "convoy effect," where shorter processes wait for a long process to complete.

#### 2. **Shortest Job First (SJF)**
- **Type:** Non-Preemptive
- **Criteria:** The process with the shortest CPU burst time in the ready queue is executed next.
- **Pros:** Minimizes average waiting time.
- **Cons:** Requires knowledge of the CPU burst time of the processes in advance.

#### 3. **Shortest Remaining Job First (SRJF)**
- **Type:** Preemptive
- **Criteria:** The process with the shortest remaining CPU burst time is executed next.
- **Pros:** Provides optimal average waiting time.
- **Cons:** More complex to implement than SJF.

#### 4. **Longest Job First (LJF)**
- **Type:** Non-Preemptive
- **Criteria:** The process with the longest CPU burst time in the ready queue is executed next.
- **Pros:** Ensures longer jobs get executed without being preempted.
- **Cons:** Can lead to poor average waiting time for shorter jobs.

#### 5. **Longest Remaining Job First (LRJF)**
- **Type:** Preemptive
- **Criteria:** The process with the longest remaining CPU burst time is executed next.
- **Pros:** Suitable for ensuring longer jobs are completed without frequent interruptions.
- **Cons:** Can be inefficient for short jobs.

#### 6. **Priority Non-Preemptive (PNP)**
- **Type:** Non-Preemptive
- **Criteria:** The process with the highest priority in the ready queue is executed next.
- **Pros:** Ensures that critical tasks are executed promptly.
- **Cons:** Lower priority processes may suffer from starvation.

#### 7. **Round Robin (RR)**
- **Type:** Preemptive
- **Criteria:** Each process is assigned a fixed time quantum and is cycled through the ready queue.
- **Pros:** Fair to all processes, ensures no starvation.
- **Cons:** Time quantum needs to be chosen carefully to balance context switch overhead and response time.

#### 8. **Highest Response Ratio Next (HRRN)**
- **Type:** Non-Preemptive
- **Criteria:** The process with the highest response ratio (waiting time + burst time) / burst time is executed next.
- **Pros:** Balances the benefits of SJF while preventing starvation.
- **Cons:** Requires computation of response ratio for each process.

### Functionalities

1. **Multiple CPU and I/O Bursts:**
   Each process can have different numbers of CPU and I/O bursts, allowing for more realistic simulation of process behavior.

2. **Gantt Chart and Timeline Chart:**
   Visual representations of the scheduling process to illustrate which processes are running at any given time.

3. **Animation of the Time Log:**
   An animated representation of how processes are handled over time, providing a dynamic view of the scheduling algorithm's operation.

4. **Comparison Metrics:**
   - **Average Completion Time:** The average time taken for all processes to complete.
   - **Turn Around Time (TAT):** The total time taken from the arrival to the completion of the process.
   - **Waiting Time:** The total time a process spends waiting in the ready queue.
   - **Response Time:** The time from the arrival of the process to the first time it gets the CPU.

### Technologies Used

- **HTML:** For structuring the web page.
- **CSS:** For styling the web page and making it visually appealing.
- **Vanilla JS:** For implementing the scheduling algorithms and handling the logic.
- **Google Charts:** For creating Gantt and Timeline charts to visualize the scheduling process and metrics.

This setup provides a robust framework for understanding and comparing different CPU scheduling algorithms through visual and interactive means.
