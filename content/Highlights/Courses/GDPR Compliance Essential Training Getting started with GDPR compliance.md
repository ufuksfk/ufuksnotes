---
description:
socialDescription:
title: GDPR Compliance Essential Training Getting started with GDPR compliance
draft: true
tags:
  - highlight/course
link: https://www.linkedin.com/learning/gdpr-compliance-essential-training-14328961
date: 2025-03-05
modified: 2025-08-21
---
Taking this course at [[2025-01#30]]

Data Privacy: The relationship between the collection and dissemination of data, technology, the public expectation of privacy, and the legal and political issues surrounding them

Consent: Any freely given, spesifict, informed agreement to the processing of personal data

Personal data: Any information relating to an identifiable natural person.

Processing: Any operation performed on personal data, such as collection, storage, alteration, retrieval, erasure ..

![[Pasted image 20250130143409.png]]

Data breaches:
[[2016]] 1093 breaches, 36 million records
[[2021]] 1222 breaches, 170 million records

**Organizations in Scope**
All sectors or industries
SMB and large enterprise

Fewer than 250 employees alleviate some records keeping obligations.

[[Personal Data in  GDPR]] is not precisely match PII under US NIST [[(PII) Personal Identifiable Information]]

25 May [[2018]], GDPR became law.

Companies must provide a **reasonable** level of protection for personal data.

2 main organizations: [[Data Controllers of GDPR]] and [[Data Processors of GDPR]]
Data controllers is data owners, their tasks:
* Compliance
* Inform
* Implement technical measures
* Written agreements with processors
* Responsible to EU citizens
Data processors, authority which process data
Task:
* Records processing operations
* Implement security mesures
* Inform of any data breach
* Responsible to controller

Joint Controllers, 2 or more controllers jointly determine why and how to process personal data

Third parties, all other parties with whom you share personal data that can process it for their purpose.

GDPR requires the appointment of a DPO for controllers and processors involved in high-risk processing activities.
The DPO may have other work responsibilities.
DPO tasks:
* Inform data subjects about their rights
* Advise
* Register of operations
* Compliance
* Handle complaints and answer questions
* Cooperate with EU and other governing agencies

Important GDPR Articles:
* Article 24: Responsibilities of the Controller
	* Implement technical and organizational measures
	* Understand the data being processed.
		* Data mapping exercise to understand why they need data
	* Implement a data protection policy
	* Develop and Approve a Code of Conduct.
* Article 28: Data processor
	* Implement security measures
		* Provide sufficient guarantees of tech and organizational measures
	* Use of subprocessors
		* Can only be done with controller's prior consent
	* Contracts with controller
		* Subject matter
		* type of data
		* nature and purpose
		* obligations of each party
	* Model clauses
		* Data transfer agreements
	* Process only data in scope
	* Logs are evidence, should be kept
* Runbooks and Processes
	* Process is a series of actions or steps in order to achieve a particular end
		* procedure, activity or operation
	* Runbook a a compilation of routine procedures and operations that the system admin or operator carries out
		* used for reference
		* electronic or physical
		* Things to include to runbook
			* System overview
			* Security and access control
			* system config
			* monitoring and alerting
			* operational tasks
			* maintenance tasks
			* failure and security procedures
			* owners and contract details
		* Security of data processing
			* Confidentiality, integrity, availability

PIA and DPIA


[[(PIA) Privacy Impact Assessment for GDPR]] analyzes how an organization handles PII
what data, how and for what purpose? and how will be destroyed

[[(DPIA) Data protection Impact Assessments for GDPR]]
security prerequisites
vendor risk assessments
self-certifications
![[Pasted image 20250130151804.png]]

Lawful basis: reason for processing that is justified by law

Data mapping exercise starts with data discovery.
What media data is stored.

Associate of Date of birth example:
Classification: confidential
Data flow: internal from US data entry to US system of record
Data use: internal only
Safeguards: Limit access to system and encrypt data

### Article 32 of GDPR: Technical Measures

Anonymize and Encrypt personal data: must be unreadable if spilled or stolen
Confidentiality, Integrity, Availability of system
https://www.cisecurity.org/controls aligned with [[ISO 27002]] and [[NIS regulation]]
Regular testing and evaluation

### Article 33 of GDPR: Notification
If a data breach is likely to result in a risk to the rights and freedom, you must notify
72 hours from becoming aware, no notification is required if it is unlikely to result a risk
Who to notify?

Your company conducts business in France and Germany. In the case of a data breach that affects all of your international customers, which notification requirements must you comply with?
	You must comply with the notification requirements of France for French customers, and Germany for German customers.

Article 15
Subject access request: they can't be charged for that. But if they request too many, controllers charge reasonable fee.
Can also request a copy of a data. Any personal data being processed. Entire period where data stored.

Article 16: Right of correction
responsibility of the controller
Data subject can request correction

Article 17: Right to be forgotten
deletion is allowed when processing no longer has a lawful basis.

Article 21: Right to object
they have right to object in most situations, but not all

Article 8: Children uder 16

Article 20: Portability
4 scenarios outlined:
1. Copies:
2. Transfer: must be ready to transfer data from one controller to another
3. Storage: 
4. Transmission: having data transmitted directly between controllers
Result of health assessment or credit score is excluded. They are outcome of personal data.

https://www.edpb.europa.eu/edpb_en

### Penalties!
DPAs = Data Protection Authorities
Monitoring and Evaluating
If they suspect, they can investigate
Imposition of Fines
Can be small and severe
Amount of fines increased in time!
Top 3 violations
1. Insufficient legal basis for data processing
2. Insufficient tech or organizational measures to ensure information security
3. Noncompliance with general data processing principles
WhatsApp Ireland Ltd fined 225 million euro for insufficient fulfillment of information obligations
Marriott International Inc fined 18 million for insufficient tech and organizations measures ..

EU GDPR is no longer applies in the UK. However, a version of GDPR lives in UK as UK GDPR

https://gdpr-info.eu/
https://gdpr.eu/