
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

