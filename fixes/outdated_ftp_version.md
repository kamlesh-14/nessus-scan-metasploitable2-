#  Outdated FTP Service Detected

##  Description:
The Nessus scan has flagged an outdated version of the FTP service running on the target (Metasploitable 2). Such outdated versions often contain multiple known vulnerabilities, including remote code execution, backdoors, or privilege escalation flaws.

##  Risk:
- Susceptible to public exploits
- Could allow **unauthorized access**
- Potential for **remote code execution** or **buffer overflow attacks**

##  Severity: High

##  Recommended Fix:
- Identify the running FTP server and its version using:
  ```bash
  telnet <target_ip> 21
