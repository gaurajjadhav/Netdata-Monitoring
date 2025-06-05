# Netdata Monitoring with Docker

## Objective
The goal of this task was to monitor system resource usage such as **CPU, memory, disk I/O, and Docker containers** using **Netdata**, a lightweight real-time monitoring tool.

---

## Tools & Technologies Used

- **Netdata** – Monitoring tool
- **Docker** – To run Netdata container
- **Web Browser** – To access the Netdata dashboard

---

## Commands Used

### 1. **Run Netdata with Docker**
```bash
docker run -d --name=netdata -p 19999:19999 --cap-add=SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata
```

**This will:**

- Download the image

- Start Netdata in detached mode

- Expose the dashboard on `http://localhost:19999`

## Steps to Complete the Task
- Start the Docker 
- Pulled and ran the official Netdata Docker image using command
```bash
docker run -d --name=netdata -p 19999:19999 --cap-add=SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata
```
- Accessed `http://localhost:19999` to view the Netdata dashboard
- Explored system performance metrics
- Captured relevant screenshots
- Created and pushed this documentation to GitHub

