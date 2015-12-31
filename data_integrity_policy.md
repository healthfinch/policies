# Data Integrity Policy

healthfinch takes data integrity very seriously. As stewards and partners of healthfinch Customers, we strive to assure data is protected from unauthorized access and that it is available when needed. The following policies drive many of our procedures and technical settings in support of the healthfinch mission of data and processing integrity.

## Data integrity Policy

Production Systems that create, receive, store, or transmit customer data (hereafter "Production Systems") must follow the following guidelines.

### Disabling non-essential services

* All Production Systems must disable services that are not required to achieve the business purpose or function of the system.

### Monitoring Log-in Attempts

* All access to Production Systems must be logged. This is done following the healthfinch Auditing Policy.

### Prevention of malware on Production Systems

* All Production Systems must have a Threat Stack agent running at set to scan system continuously to assure no malware is present. Detected malware is evaluated and removed.
* All outbound network connections from Production Systems must be whitelisted, to prevent exfiltration of data by malware
* All Production Systems are to only be used for healthfinch business needs.

### Patch Management

* Patches, application, and system OS versions are kept up to date at all times. New versions are tested.
* Seccurity patches on a OS vendor (Canonical Ubuntu) approved list are automatically applied within 24 hours of being available.
* Administrators subscribe to mailing lists to assure up to date on current version of all healthfinch managed software on Production Systems.

### Intrusion Detection and Vulnerability Scanning

* Production Systems are monitored using Threat Stack IDS systems. Suspicious activity is logged and alerts are generated.
* Vulnerability scanning of Production Systems must occur on a predetermined, regular basis, no less than annually. Scans are reviewed by Security Officer, with defined steps for risk mitigation, and retained for future reference.

### Production System Security

* System, network, and server security is managed and maintained by the CTO and Security Officer.
* Up to date system lists and architecture diagrams are kept for all Production environments.
* Access to Production Systems is controlled using two-factor authentication, including a PKCS11-compliant smart card containing a private key assigned to an operator

### Production Data Security

* Reduce the risk of compromise of Production Data.
* Implement and/or review controls designed to protect Production Data from improper alteration or destruction.
* Ensure that Confidential data is stored in a manner that supports user access logs and automated monitoring for potential security incidents.
* All Production Data at rest is stored on encrypted volumes using NIST-standard AES 256 encryption.

### Transmission Security

* All data transmission is encrypted end to end using NIST-standard TLS 1.2 transport-level encryption. Encryption is terminated at the network end point, and is re-encrypted through to the application.
* Encryption keys and machines that generate keys are protected from unauthorized access.
* Encryption keys are limited to use for one year and then must be regenerated.
* In the case of healthfinch provided APIs, we provide mechanisms to assure persons or systems sending or receiving data are authorized to send and save data.
* System logs of all transmissions of Production Data access. These logs must be available for audit.

### Applicable Standards from the HITRUST Common Security Framework

* 10.b - Input Data Validation

### Applicable Standards from the HIPAA Security Rule

* 164.308(a)(8) - Evaluation

### Applicable Standards from the SOC2 Trust Services Principles
