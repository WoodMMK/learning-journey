# Web Application Penetration Testing Notes

## 📌 Description
This file contains my notes, resources, and tools related to Web App Pentest including wordlists works in my solved CTF challenges, tools, and techniques (cheatsheet).

## 🔹 Enumeration & Information Gathering
### Tools & Techniques
- **Nmap**: Scan for open ports and services
  ```bash
  # normal scan on 100 ports
  nmap <targetIP> 

  # specify port -p portnum1,portnum2,...
  ```
- **Gobuster **: Directory and file enumeration
  ```bash
  gobuster dir -u http://<targetIP> -w /usr/share/wordlists/dirb/common.txt
  ```

## 🔹 Common Wordlists
- [Seclist's](https://github.com/danielmiessler/SecLists/tree/master)
- [rockyou](https://github.com/praetorian-inc/Hob0Rules/blob/master/wordlists/rockyou.txt.gz)

## 🔹 SQL Injection
### Manual Testing
- Find the vuln & exploit (look for SQLi vuln types)
- find dbms -> table_name and  its structures -> dump data

### automated testing:
**SQLMap**
  ```bash
  sqlmap -u "http://target.com/login.php?id=1" --dbs --batch
  ```

## 🔹 Resources & References
### 📚 Learning Platforms
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)
- [OWASP Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [HackTricks](https://book.hacktricks.xyz/)
- [TryHackMe - Web Fundamentals](https://tryhackme.com/room/webfundamentals)
- [PentesterLab](https://pentesterlab.com/)

### 📜 Cheat Sheets
- [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings)
- [SecLists Wordlists](https://github.com/danielmiessler/SecLists)
- [GTFOBins](https://gtfobins.github.io/) (no writeups yet)

## 🛠️ Tools to Install
```bash
sudo apt install gobuster sqlmap 
```

---
💡 **Updates will be added soon as I learning!**
