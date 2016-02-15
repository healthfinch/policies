# Introduction

healthfinch, Inc ("healthfinch") is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it receives, maintains, processes and/or transmits on behalf of its Customers. As providers of compliant, hosted infrastructure used by health technology vendors, developers, designers, agencies, custom development shops, and enterprises, healthfinch strives to maintain compliance, proactively address information security, mitigate risk for its Customers, and assure known breaches are completely and effectively communicated in a timely manner. The following documents address core policies used by healthfinch to maintain compliance and assure the proper protections of infrastructure used to store, process, and transmit ePHI for healthfinch Customers.

healthfinch provides secure and compliant cloud-based software. This hosted software falls into the broad category of **Software as a Service (SaaS)**.

## Compliance Inheritance

healthfinch signs business associate agreements (BAAs) with its Customers. These BAAs outline healthfinch obligations and Customer obligations, as well as liability in the case of a breach. In providing services and managing security configurations that are a part of the technology requirements that exist in HIPAA and HITECH regulations, as well as future compliance frameworks, healthfinch manages various aspects of compliance for Customers. The aspects of compliance that healthfinch manages for Customers are inherited by Customers, and healthfinch assumes the risk associated with those aspects of compliance. In doing so, healthfinch helps Customers achieve and maintain compliance, as well as mitigates Customers risk.

Certain aspects of compliance cannot be inherited. Because of this, healthfinch Customers, in order to achieve full compliance or HITRUST Certification, must implement certain organizational policies. These policies and aspects of compliance fall outside of the services and obligations of healthfinch.

Below are mappings of HIPAA Rules to healthfinch controls and a mapping of what Rules are inherited by Customers.

## healthfinch Operational Concepts

The physical infrastructure environment is hosted at [AWS](ttps://d0.awsstatic.com/whitepapers/Security/AWS_Security_Whitepaper.pdf). The network components and supporting network infrastructure is contained within AWS infrastructure and managed by AWS. healthfinch does not have physical access into the network components. The healthfinch environment consists of Nginx web servers, Unicorn (Ruby on Rails) application servers, PostgreSQL and Redis database servers, Sumo Logic log monitoring and collection services, Chef hosted configuration management services, Threatstack IDS services, Datadog system and performance monitoring, Linux Ubuntu bastion host, and developer tool servers running on Linux Ubuntu.

Within the healthfinch Platform, all data transmission is encrypted and all hard drives are encrypted so data at rest is also encrypted to NIST-recommended standards (TLS 1.2 and AES 256 respectively); this applies to all servers, hosting application servers, databases, APIs, log servers, etc. healthfinch assumes all data *may* contain ePHI, even though our Risk Assessment does not indicate this is the case, and provides appropriate protections based on that assumption.

The bastion host and Nginx web server is externally facing and accessible via the Internet. The database servers, where the ePHI resides, are located on the internal healthfinch network and can only be accessed directly over an SSH connection through the bastion host. The access to the internal database is restricted to a limited number of personnel and strictly controlled to only those personnel with a business justified reason. Remote access to the internal servers is not accessible except through the load balancers and bastion host.
