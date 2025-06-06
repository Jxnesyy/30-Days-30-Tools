# Day 5 – Nmap

## Scan Summary:
Target: scanme.nmap.org (45.33.32.156)

### Open Ports:
- 22/tcp – SSH (remote login)
- 80/tcp – HTTP (web server)
- 9929/tcp – Nping Echo
- 31337/tcp – Elite (possible backdoor)

### Observations:
- 427/tcp (svrloc) was **filtered**, indicating possible firewall or intrusion prevention.
- 31337 is a well-known “hacker” port — potentially a honeypot or easter egg.

### What I Learned:
- How to detect open, closed, and filtered ports.
- How Nmap identifies services and basic firewall behavior.
- Using Nmap effectively is critical in real-world red team operations.

## Command Used:
```bash
nmap scanme.nmap.org -oN nmap_scan_output.txt
