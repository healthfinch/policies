# Data Management Policy

Data backup is an important part of the day-to-day operations of healthfinch. To protect the confidentiality, integrity, and availability of ePHI, both for healthfinch and healthfinch Customers, completes backups are done daily to assure that data remains available when it needed and in case of disaster.

Violation of this policy and its procedures by workforce members may result in corrective disciplinary action, up to and including termination of employment.

## Backup Policy and Procedures

1. Perform daily snapshot backups of all systems that process, store, or transmit ePHI for healthfinch Customers, or which produce auditable data as a result of services provided to Customers
2. healthfinch Ops Team, lead by the CTO, is designated to be in charge of backups.
3. Dev Ops Team members are trained and assigned assigned to complete backups and manage the backup media.
4. Document backups 
	* Name of the system
	* Date & time of backup
	* Where backup stored (or to whom it was provided)
5. Securely encrypt stored backups in a manner that protects them from loss or environmental damage.
6. Store at least one copy of backups in a manner that prevents it from sharing a single point of failure with its source of record, including colocation
7. Regularly test backups and document that files have been completely and accurately restored from the backup media (currently daily)

### Applicable Standards from the HITRUST Common Security Framework

* 01.v - Information Access Restriction

### Applicable Standards from the HIPAA Security Rule

* 164.308(a)(7)(ii)(A) - Data Backup Plan
* 164.310(d)(2)(iii) - Accountability
* 164.310(d)(2)(iv) - Data Backup and Storage

### Applicable Standards from the SOC2 Trust Services Principles
