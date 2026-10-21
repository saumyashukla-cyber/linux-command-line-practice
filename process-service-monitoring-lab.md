
# Process and Service Monitoring Lab

## Objective
To practise monitoring running processes and checking Linux service status.

## Environment
- Operating System: Kali Linux

## Tasks

### 1. View Running Processes
Command: `ps aux`

Purpose: To display running processes and their details.

### 2. Monitor System Processes
Command: `top`

Purpose: To monitor processes and system resource usage in real time.

### 3. Check SSH Service Status
Command: `systemctl status ssh`

Purpose: To inspect the current status of the SSH service.

### 4. List Running Services
Command: `systemctl list-units --type=service --state=running`

Purpose: To list currently running system services.


## Observations

### 1. Running Processes
- Executed `ps aux` to display running processes.
- Observed process IDs (PIDs), usernames, CPU usage, memory usage, and command names.
- Identified system processes such as `systemd` and `NetworkManager`.

### 2. Real-Time Monitoring
- Executed `top` to monitor running processes and system resource usage in real time.
- Observed CPU usage, memory usage, total tasks, and process details.
- Noted that CPU usage was approximately 98% idle during the observation.

### 3. SSH Service Status
- Executed `systemctl status ssh`.
- Observed that the SSH service was inactive (dead).
- The service was loaded but disabled, meaning it was not configured to start automatically.

### 4. Running Services
- Executed `systemctl list-units --type=service --state=running`.
- Observed the services currently running on the system.



## Conclusion
This lab practises Linux process monitoring and service inspection.
