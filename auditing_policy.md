
# Auditing Policy

healthfinch shall audit access and activity of electronic protected health information (ePHI) applications and systems in order to ensure compliance. The Security Rule requires healthcare organizations to implement reasonable hardware, software, and/or procedural mechanisms that record and examine activity in information systems that contain or use ePHI. Audit activities may be limited by application, system, and/or network auditing capabilities and resources. healthfinch shall make reasonable and good-faith efforts to safeguard information privacy and security through a well-thought-out approach to auditing that is consistent with available resources.

It is the policy of healthfinch to safeguard the confidentiality, integrity, and availability of applications, systems, and networks. To ensure that appropriate safeguards are in place and effective, healthfinch shall audit access and activity to detect, report, and guard against:

* Network vulnerabilities and intrusions;
* Breaches in confidentiality and security of patient protected health information;
* Performance problems and flaws in applications;
* Improper alteration or destruction of ePHI;
* Out of date software and/or software known to have vulnerabilities.

This policy applies to all healthfinch systems that store, transmit, or process ePHI.

# Auditing Policies

1. Responsibility for auditing information system access and activity is assigned to healthfinch’s Security Officer. The Security Officer shall:
	* Assign the task of generating reports for audit activities to the workforce member responsible for the application, system, or network;
	* Assign the task of reviewing the audit reports to the workforce member responsible for the application, system, or network, the Privacy Officer, or any other individual determined to be appropriate for the task;
	* Organize and provide oversight to a team structure charged with audit compliance activities (e.g., parameters, frequency, sample sizes, report formats, evaluation, follow-up, etc.).
	* All connections to healthfinch are monitored. Access is limited to certain services, ports, and destinations. Exceptions to these rules, if created, are reviewed on an annual basis. 
2. healthfinch’s auditing processes shall address access and activity at the following levels listed below. 
	* User: User level audit trails generally monitor and log all commands directly initiated by the user, all identification and authentication attempts, and data and services accessed.
	* Application: Application level audit trails generally monitor and log all user activities, including data accessed and modified and specific actions.
	* System: System level audit trails generally monitor and log user activities, applications accessed, and other system defined specific actions. healthfinch utilizes file system monitoring of key system files to assure the integrity of file system data.
	* Network: Network level audit trails generally monitor information on what is operating, penetrations, and vulnerabilities.
3. healthfinch shall log all incoming and outgoing traffic to into and out of its environment. This includes all successful and failed attempts at data access and editing. Data associated with this data will include origin, destination, time, and other relevant details that are available to healthfinch.
4. healthfinch utilizes Threat Stack to scan all systems for malicious and unauthorized activity on a continuous basis at the syscall level.
5. healthfinch leverages process monitoring tools throughout its environment, for proactive response to failure and passive collection of performance statistics using a centralized metrics collection tool
6. healthfinch shall identify “trigger events” or criteria that raise awareness of questionable conditions of viewing of confidential information. The “events” may be applied to the entire healthfinch Platform or may be specific to a Customer, partner, business associate, Platform Add-on or application (See Listing of Potential Trigger Events below).
7. In addition to trigger events, healthfinch utilizes OSSEC log correlation functionality to proactively identify and enable alerts based on log data.
8. Logs are reviewed weekly by Security Officer. 
9. healthfinch’s Security Officer and Privacy Officer are authorized to select and use auditing tools that are designed to detect network vulnerabilities and intrusions. Such tools are explicitly prohibited by others, including Customers and Partners, without the explicit authorization of the Security Officer. These tools may include, but are not limited to:
	* Scanning tools and devices;
	* Password cracking utilities;
	* Network “sniffers.”
	* Passive and active intrusion detection systems.
10. The process for review of audit logs, trails, and reports shall include:
	* Description of the activity as well as rationale for performing the audit.
	* Identification of which healthfinch workforce members will be responsible for review (workforce members shall not review audit logs that pertain to their own system activity).
	* Frequency of the auditing process.
	* Determination of significant events requiring further review and follow-up.
	* Identification of appropriate reporting channels for audit results and required follow-up.
13. Vulnerability testing software may be used to probe the network to identify what is running (e.g., operating system or product versions in place), whether publicly-known vulnerabilities have been corrected, and evaluate whether the system can withstand attacks aimed at circumventing security controls.
	* Testing may be carried out internally or provided through an external third-party vendor. Whenever possible, a third party auditing vendor should not be providing the organization IT oversight services (e.g., vendors providing IT services should not be auditing their own services - separation of duties).
	* Testing shall be done on a routine basis, currently monthly.
14. Software patches and updates will be applied to all systems in a timely manner. Vendor-approved security patches are applied automatically withing 24 hours of being made available. In the case of routine updates, they will be applied after thorough testing.

## Review and Reporting of Audit Findings

1. Audit information that is routinely gathered must be reviewed in a timely manner, by the responsible workforce member(s). Daily reviews of summary reports are preferred if possible, otherwise monthly reviews are expected.
2. Significant findings shall be reported immediately in a written format. healthfinch’s security incident response form may be utilized to report a single event.
3. Routine findings shall be reported to the sponsoring leadership structure in a written report format.
4. Reports of audit results shall be limited to internal use on a minimum necessary/need-to-know basis. Audit results shall not be disclosed externally without administrative and/or legal counsel approval.
5. Security audits constitute an internal, confidential monitoring practice that may be included in healthfinch’s performance improvement activities and reporting. Care shall be taken to ensure that the results of the audits are disclosed to administrative level oversight structures only and that information which may further expose organizational risk is shared with extreme caution. Generic security audit information may be included in organizational reports (individually-identifiable ePHI shall not be included in the reports).
6. Whenever indicated through evaluation and reporting, appropriate corrective actions must be undertaken. These actions shall be documented and shared with the responsible workforce members, Customers, and/or Partners.

## Audit Log Security Controls and Backup

7. Audit logs shall be protected from unauthorized access or modification, so the information they contain will be made available only if needed to evaluate a security incident or for routine audit activities as outlined in this policy.
8. All audit logs are encrypted in transit and at rest to control access to the content of the logs. 
9. Audit logs shall be stored on a separate, centralized system to minimize the impact auditing may have on the privacy system and to prevent access to audit trails by those with system administrator privileges. This is done to apply the security principle of “separation of duties” to protect audit trails from hackers.

## External Audits of Information Access and Activity

1. Prior to contracting with an external audit firm, healthfinch shall:
	* Outline the audit responsibility, authority, and accountability;
	* Choose an audit firm that is independent of other organizational operations;
	* Ensure technical competence of the audit firm staff;
	* Require the audit firm’s adherence to applicable codes of professional ethics;
	* Obtain a signed HIPAA business associate agreement;
	* Assign organizational responsibility for supervision of the external audit firm.

## Retention of Audit Data

1. Audit logs shall be maintained based on organizational needs. There is no standard or law addressing the retention of audit log/trail information. Retention of this information shall be based on:
A. Organizational history and experience.
B. Available storage space.
1. Reports summarizing audit activities shall be retained for a period of six years.
3. Log data is currently retained and readily accessible for a 90-day period. Beyond that, log data is available via cold backup. 

## Potential Trigger Events

* High risk or problem prone incidents or events.
* Business associate, customer, or partner complaints.
* Known security vulnerabilities.
* Atypical patterns of activity.
* Failed authentication attempts.
* Remote access use and activity.
* Activity post termination.
* Random audits.

### Applicable Standards from the HITRUST Common Security Framework

* 0.a Information Security Management Program
* 01.a Access Control Policy
* 01.b User Registration
* 01.c Privilege Management
* 09.aa Audit Logging
* 09.ac Protection of Log Information
* 09.ab - Monitoring System Use
* 06.e - Prevention of Misuse of Information

### Applicable Standards from the HIPAA Security Rule

* 45 CFR ¬ß 164.308(a)(1)(ii)(D) - Information System Activity Review
* 45 CFR ¬ß 164.308(a)(5)(ii)(B) & (C) - Protection from Malicious Software & Log-in Monitoring
* 45 CFR ¬ß 164.308(a)(2) - HIPAA Security Rule Periodic Evaluation
* 45 CFR ¬ß 164.312(b) - Audit Controls
* 45 CFR ¬ß 164.312(c)(2) - Mechanism to Authenticate ePHI
* 45 CFR ¬ß 164.312(e)(2)(i) - Integrity Controls

### Applicable Standards from the SOC2 Trust Services Principles

* Common Controls (CC) 2.2
