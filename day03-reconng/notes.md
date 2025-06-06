# Day 3 - Recon-ng
**Target:** tesla.com  
**Workspace:** tesla  
**Modules Used:**
- recon/domains-hosts/bing_domain_web
- recon/domains-hosts/hackertarget
- recon/hosts-hosts/resolve
- recon/domains-contacts/whois_pocs

---

## 🧠 Subdomains & Hosts Discovered
- shop.eu.tesla.com → 205.234.27.221
- model3.tesla.com → 205.234.27.221
- events.tesla.com → 13.111.47.195
- marketing.tesla.com → 13.111.47.196
- emails.tesla.com + 10+ related email infra subdomains
- vpn1.tesla.com → 8.45.124.215
- monitoring.tesla.com → 23.202.44.211
- gpgw + ptr DNS mapped domains

✅ Total Hosts Discovered: **37**

---

## 📧 WHOIS Contacts Extracted
- Cheri Lewis-Carey (chelewis@tesla.com)
- Jian Gu (jiangu@tesla.com)
- Mahesh Desai (mahdesai@tesla.com)
- Seyed Jafarinejad (sejafarinejad@tesla.com)
- Terry Chi (tchi@tesla.com)

✅ Total WHOIS Contacts: **10**

---

## 🧾 CLI Commands
```bash
recon-ng
workspaces create tesla
modules load recon/domains-hosts/bing_domain_web
options set SOURCE tesla.com
run
...
