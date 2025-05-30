# Task 4: Setup and Use a Firewall on Windows

## ✅ Objective
To configure and test basic firewall rules using Windows Defender Firewall.

## 🛠 Tools Used
- Windows Defender Firewall with Advanced Security  
- PowerShell  
- Telnet Client  

## 📌 Steps performed
- Opened Windows Firewall using `wf.msc`.
- Created an inbound rule to block TCP traffic on port 23 (Telnet).
- Verified the block using PowerShell:
  ```powershell
  Test-NetConnection -ComputerName localhost -Port 23
 Result: TcpTestSucceeded: False
 → Port 23 was successfully blocked.
- Removed the rule and retested the connection.
 Result: TcpTestSucceeded: True
→ Port 23 was successfully unblocked.

---

## 📂 Files in this Repository
### ▶️  [`Documents/`](./Documents/)
- Task 4-Setup and Use a Firewall on Windows: Word document containing the process
- Screenshots regarding the task

---

## ✅ Outcome
This task demonstrated how to block and allow network traffic using Windows Firewall. PowerShell was used to test the rule's effectiveness. By creating, verifying, and removing a rule, a better understanding of firewall traffic filtering was achieved.
