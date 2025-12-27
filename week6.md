## Week 6 – Performance Evaluation & Analysis

### Performance Evaluation and Analysis
This week focuses on evaluating the performance of the Linux server operating system under different workloads. Performance evaluation involves measuring how system resources such as CPU, memory, disk I/O, and network bandwidth are used during normal operation and under increased load. Performance analysis is then used to interpret this data, identify system bottlenecks, and understand how configuration choices impact overall system efficiency, stability, and responsiveness.

### Testing Approach

Performance testing is carried out to evaluate how the Linux server operating system behaves under different workloads and to identify potential performance bottlenecks. All tests are conducted by connecting remotely to the server via SSH from the workstation, ensuring the server remains headless and is administered using command-line tools only.

System performance is monitored using standard Linux utilities such as `top`, `htop`, `free`, `df`, `iostat`, `vmstat`, and `uptime`, along with network tools including `ping` and `iperf`. Performance data is collected during baseline (idle) conditions and during application load testing, with outputs recorded through terminal screenshots and logged results.

Each test is executed three times, and average values are calculated to improve the accuracy and reliability of the performance analysis.

