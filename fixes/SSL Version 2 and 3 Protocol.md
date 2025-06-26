#  SSL Version 2 and 3 Protocol Detected

##  Description:
The scan detected that the server supports outdated and insecure versions of the SSL protocol — **SSLv2** and **SSLv3**.

These protocols are deprecated and contain serious vulnerabilities (like POODLE for SSLv3), which make encrypted communication susceptible to interception or tampering.

##  Risk:
- Weak cryptographic negotiation
- Susceptible to **Man-in-the-Middle (MitM)** attacks
- Enables **downgrade attacks**

##  Severity: High

##  Recommended Fix:
- Disable SSLv2 and SSLv3 in the service configurations (e.g., Apache, Nginx, Postfix, etc.)
- Ensure only **TLS 1.2 or TLS 1.3** are enabled

### Example (for Apache):
```bash
SSLProtocol All -SSLv2 -SSLv3
