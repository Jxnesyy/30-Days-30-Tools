Day 7 - Recon Report: tesla.com
🔎 1. Domain Info
Registrar: MarkMonitor Inc.

Registrant: Tesla, Inc.

Creation Date: 2003-06-02

Name Servers:

NS-1108.AWSDNS-10.ORG

NS-1649.AWSDNS-14.CO.UK

NS-372.AWSDNS-46.COM

NS-929.AWSDNS-52.NET

🌍 2. DNS Records
A Record: 104.111.227.110 (Akamai CDN)

MX:

aspmx.l.google.com

alt1.aspmx.l.google.com

TXT:

v=spf1 include:_spf.google.com include:amazonses.com -all

dmarc.tesla.com "v=DMARC1; p=reject; rua=mailto:dmarc-reports@tesla.com"

NS:

Amazon AWS Nameservers (see above)

📬 3. Email Harvested
press@tesla.com

ir@tesla.com

support@tesla.com

(No exposed personal emails found in scans)

🌐 4. Subdomains (Top 5–10)
api.tesla.com

shop.tesla.com

investor.tesla.com

energy.tesla.com

fleet-api.tesla.com

staging.tesla.com

downloads.tesla.com

auth.tesla.com

(Sourced via crt.sh, Sublist3r, Spiderfoot)

🧰 5. Shodan Results
Open Ports: 80 (HTTP), 443 (HTTPS), 8080, 8443

Detected Devices:

Web Application Firewalls (Cloudflare)

Reverse proxies on some API endpoints

CDN-based load balancing (Akamai)

Location IPs:

US-based Akamai edge servers (CDN obfuscation active)

🕸️ 6. OSINT Correlation
Technologies:

Cloudflare (WAF, DNS)

Akamai (CDN)

AWS (backend services)

Nginx (reverse proxy)

Potential Leaks:

GitHub employee contributions referencing internal dev/staging endpoints

Public LinkedIn profiles listing internal software/tools

JS files with commented-out old endpoints

📌 Summary
Tesla demonstrates a high level of security awareness, leveraging CDNs, WAFs, and segregated environments. However, exposed subdomains, legacy API endpoints, and OSINT metadata may still aid targeted reconnaissance. Continued passive monitoring and DNS tracking advised.
