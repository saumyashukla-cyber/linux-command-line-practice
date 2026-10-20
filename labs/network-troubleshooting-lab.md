*Linux Network Troubleshooting Lab*

Objective
Practise basic Linux networking commands used to inspect network configuration, test connectivity, and view network connections.

Environment
- Operating System: Kali Linux
- Tool: Linux terminal

1. Check IP Address Configuration

Command:
```bash
ip addr
```

Purpose: Displays network interfaces and their IP addresses.
<img width="1030" height="507" alt="image" src="https://github.com/user-attachments/assets/9ea5299f-1978-43cd-90e0-5bc58af43e35" />



2. Check the Routing Table

Command:
```bash
ip route
```

Purpose: Displays routing information, including the default gateway when configured.
<img width="921" height="178" alt="image" src="https://github.com/user-attachments/assets/5c329563-2109-4db5-9134-bcdd133f198f" />



3. Test Network Connectivity

Command:
```bash
ping -c 4 127.0.0.1
```

Purpose: Tests connectivity to the local loopback address.
<img width="750" height="257" alt="image" src="https://github.com/user-attachments/assets/f08ad7c2-77df-423c-bd58-10d1d4f5b4a3" />



4. Inspect Network Connections

Command:
```bash
ss -tuln
```

Purpose: Lists listening TCP and UDP sockets.

![TCP Network Connections](/home/kali/Downloads/Screenshot_2026-10-15_11_55_42.png)


Troubleshooting Checklist
- Check whether the network interface is up.
- Verify the IP address and subnet configuration.
- Inspect the routing table.
- Test connectivity and compare results.
- Review listening ports when investigating a service.

Security Relevance
Basic network inspection helps IT Support teams troubleshoot connectivity and helps security analysts understand listening services and network configuration.

Results
Record the actual command output and observations after running each command in your Linux lab.




