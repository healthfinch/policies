# Configuration Management Policy

healthfinch standardizes and automates configuration management through the use of the Chef configuration management system as well as documentation of all changes to production systems and networks. Chef automatically configures all healthfinch systems according to established and tested policies, and is used as part of our Disaster Recovery plan and process.

## Configuration Management

1. Chef is used to standardize and automate configuration management.
2. Threat Stack agents scan systems continuously. These scans capture file system changes and also unauthorized or malicious activity at the syscall level.
3. No systems are deployed into healthfinch environments without approval of the healthfinch CTO.
4. All changes to production systems, network devices, and firewalls are approved by the healthfinch CTO before they are implemented. Additionally, all changes are tested before they are implemented in production.
5. An up-to-date inventory of systems is maintained using Google spreadsheets and architecture diagrams hosted on Google Apps, Confluence wiki, and in a version control repository of an access-controlled private documenation web site. All systems are categorized as production and utility to differentiate based on criticality.
6. Clocks are synchronized across all systems using NTP.
7. All software and systems are tested using unit tests and end to end tests.
8. All committed code is reviewed using pull requests (on Github) to assure software code quality and proactively detect potential security issues in development.
9. healthfinch utilizes qa and staging environments that mirror production to assure proper function.
10. healthfinch also deploys environments locally using Vagrant to assure functionality before moving to staging or production.
11. healthfinch schedules production deployment continuously, as soon as a feature has been validated and tested in a lower environment. Small independent changes minimizes the risk of instability due to complex interdependencies.
12. All formal change requests require unique ID and authentication and are made in an auditable change request system, Pivotal Tracker.

### Applicable Standards from the HITRUST Common Security Framework

* 06 - Configuration Management

### Applicable Standards from the HIPAA Security Rule

* 164.310(a)(2)(iii) Access Control & Validation Procedures

### Applicable Standards from the SOC2 Trust Services Principles
