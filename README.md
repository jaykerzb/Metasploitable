# Penetration Testing with Metasploitable and Vulnerability Scanning with Nessus
- Below contains the information gathered and exploited in my efforts in Metasploitable.
- Attached above are my Nessus Vulnerability Reports in a High Level and Detailed format.

### Initial Recon
- Upon initial inspection, I decided to start with an Nmap scan of the system, enumerating all open ports and services, alongside the version of services to find any outdated or vulnerable versions.
- My results below:

<img width="706" alt="NmapScan" src="https://github.com/user-attachments/assets/b0f6df1d-f879-486f-8937-5316c2c78841">

I found that the version of ftp running was delivered with a backdoor vulnerability that I would then exploit: https://nvd.nist.gov/vuln/detail/CVE-2011-2523
### Exploitation
- After discovering the vulnerability, I went to work to use the backdoor left for me.
- I entered the username totalynotabackdoor:). The smiley face ":)" at the end of the username is what activates the backdoor. It allows a user to open a listening port on 6200 to access the machine with no login necessary, as shown below:
<img width="718" alt="RunningExploit" src="https://github.com/user-attachments/assets/72f48182-c1eb-4525-9031-06e2fe022ba6">
<img width="723" alt="Infiltration" src="https://github.com/user-attachments/assets/2fd97c74-b970-4341-9072-37d70ba5d72e">

After completing this, I had full telnet access to the remote system, allowing me to do whatever I wanted with the machine.
