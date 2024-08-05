# Penetration Testing with Metasploitable and Vulnerability Scanning with Nessus
- Below contains the information gathered and exploited in my efforts in Metasploitable.

### Initial Recon
- Upon initial inspection, I decided to start with an Nmap scan of the system, enumerating all open ports and services, alongside the version of services to find any outdated or vulnerable versions.
- My results below:
<img width="706" alt="NmapScan" src="https://github.com/user-attachments/assets/b0f6df1d-f879-486f-8937-5316c2c78841">
_I found that the version of ftp running was delivered with a backdoor vulnerability that I would then exploit_
[link](https://nvd.nist.gov/vuln/detail/CVE-2011-2523)
