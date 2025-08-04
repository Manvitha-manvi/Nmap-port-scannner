# 🔍 Nmap Port Scanner — Cyber Security Internship Task 1

1. Overview
This project was completed as part of my Cyber Security Internship. The goal was to learn how to use **Nmap** to scan a local network, identify open ports, and understand their security implications.

2. What I Did
- Found my IP (`192.168.56.1`) using `ipconfig`
- Scanned the entire subnet `192.168.56.0/24` using:
  ```bash
  nmap -sS 192.168.56.0/24 -oN scan_results.txt
Nmap found 1 host with 4 open ports
Saved the results in scan_results.txt

3. Scan Summary
IP Address	Open Ports	Services
192.168.56.1	135, 139, 445, 8090	msrpc, netbios-ssn, microsoft-ds, opsmessaging

4. Security Insights
135/139/445 are Windows ports often targeted by ransomware (e.g., WannaCry)
8090 is commonly used by web/dev servers — risky if exposed publicly

5. Files in Repo
scan_results.txt – Nmap output
README.md – Documentation

6. What I Learned
   1.How to perform a TCP SYN scan with Nmap
   2.How to analyze open ports and their associated services
   3.The importance of securing unused or sensitive ports

7. Conclusion
This task gave me hands-on experience in basic network reconnaissance and strengthened my understanding of network exposure — a key skill in cybersecurity.
