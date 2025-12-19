
# Week 3 – Application Selection for Performance Testing

## 1. Introduction
This week focuses on selecting suitable applications and workloads for performance testing on the Ubuntu Server environment. The aim is to choose applications that represent different workload types in order to evaluate CPU, memory, disk I/O, and network performance. This week is focused on planning and documentation only, with installation and execution scheduled for later weeks.

---

## 2. Application Selection Matrix
The following table lists the selected applications and workloads along with their workload type, primary system resource tested, and justification for selection.

| Application / Tool | Workload Type | Primary Resource Tested | Justification |
|--------------------|---------------|-------------------------|---------------|
| stress-ng (CPU) | CPU-intensive | CPU | Used to generate high CPU load and evaluate processor performance under stress |
| stress-ng (Memory) | RAM-intensive | Memory | Allocates and uses large amounts of RAM to analyse memory behaviour |
| dd | I/O-intensive | Disk | Used to test disk read/write speed and storage throughput |
| iperf3 | Network-intensive | Network | Measures network bandwidth and throughput between systems |
| ping | Network latency test | Network | Measures network latency and packet loss |
| Simple HTTP service (optional) | Server application | CPU / Network | Represents a basic server workload handling client requests |

These applications were selected because they provide coverage of the main system resources and allow controlled and repeatable performance testing.

---

## 3. Installation Documentation (SSH-Based Installation)
All applications will be installed on the Ubuntu Server using SSH-based remote administration from the workstation. Installation will be carried out using the system package manager.

Planned installation commands include:
sudo apt update
sudo apt install stress-ng
sudo apt install iperf3

The `dd` and `ping` commands are included by default in Ubuntu Server and do not require additional installation. Any installation steps will be performed remotely to maintain a headless server environment.

---

## 4. Expected Resource Profiles
Before execution, the expected system resource usage for each application is documented below.

| Application | Expected Resource Usage |
|------------|--------------------------|
| stress-ng (CPU) | High CPU usage across one or more processor cores |
| stress-ng (Memory) | High RAM usage due to memory allocation and stress |
| dd | High disk read/write activity with minimal CPU usage |
| iperf3 | High network bandwidth usage |
| ping | Low bandwidth usage with focus on latency measurement |
| HTTP service | Moderate CPU and network usage depending on request load |

These expected profiles provide a baseline understanding of how each workload should affect system performance.

---

## 5. Monitoring Strategy
System performance will be monitored remotely from the workstation using SSH while workloads are running on the server. Different monitoring tools will be used depending on the workload type.

- CPU and memory usage will be monitored using `top` and `htop`
- Overall system activity will be monitored using `vmstat`
- Disk input/output activity will be monitored using `iostat`
- Network bandwidth usage will be monitored using `iperf3` and interface statistics
- Network latency will be monitored using `ping`

Performance data will be collected during baseline and workload execution to enable comparison and identification of performance bottlenecks in later weeks.

---

## 6. Reflection
This week successfully identified suitable applications and workloads for performance testing. By selecting workloads that represent different system resource demands and documenting installation steps, expected resource usage, and monitoring strategies, a strong foundation has been created for practical performance evaluation and optimisation in subsequent weeks.


