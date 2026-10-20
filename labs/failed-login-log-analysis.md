# Linux Failed Login Log Analysis

## 1. Project Overview
This project explores how Linux authentication logs can be used to investigate failed login attempts.

## 2. Objective
- Understand authentication logs.
- Identify failed login events.
- Practise filtering log entries.
- Document findings in an incident-investigation format.

## 3. Environment
- Operating System: Kali Linux
- Tools: Terminal, grep, journalctl (where available)

## 4. Log Sources
Depending on the Linux distribution and logging configuration, authentication events may be recorded in:
- `/var/log/auth.log`
- The systemd journal

## 5. Investigation Steps

### Step 1: Check whether the authentication log exists
```bash
ls -l /var/log/auth.log
```


### Step 2: Search for failed login messages
If the log file exists:
```bash
grep -i "failed" /var/log/auth.log
```

### Step 3: Search SSH authentication failures
```bash
grep -i "failed password" /var/log/auth.log
```

### Step 4: Check authentication events in the system journal
Where supported and permitted:
```bash
sudo journalctl | grep -i "failed password"
```

## 6. Investigation Checklist
- Identify the event timestamp.
- Identify the source IP address, if recorded.
- Identify the targeted username.
- Count repeated failures.
- Check for successful logins around the same time.
- Determine whether further investigation is needed.

## 7. Findings
Record actual results from the lab here. Do not invent event counts, IP addresses, or conclusions.

## 8. Security Relevance
Repeated authentication failures can indicate mistyped credentials, misconfigured services, or possible password-guessing activity. Additional evidence is required before classifying activity as malicious.

## 9. Conclusion
This lab demonstrates basic authentication-log filtering and investigation documentation.
