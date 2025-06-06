# Day 6 – Nikto

## Target: testphp.vulnweb.com

Nikto is a web server scanner that checks for:
- Outdated server software
- Misconfigurations
- Dangerous files and directories

### Key Findings:
- Potentially sensitive files exposed
- Apache version info visible
- SSL and HTTP headers not securely configured

### Command Used:
```bash
nikto -h http://testphp.vulnweb.com -o nikto_report.txt
