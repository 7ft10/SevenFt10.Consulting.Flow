# Audit Logs

{% hint style="success" %}
_**We use this to** ... **so that we can** ..._
{% endhint %}

## Log management <a href="#template-auditlogs-logmanagement" id="template-auditlogs-logmanagement"></a>

Log management is the process of generating, analyzing, and storing logs. Organizations that develop best practices in log management will get timely analysis of their security profile for security operations, ensure that logs are kept in sufficient detail for the appropriate period of time to meet audit and compliance requirements, and have reliable evidence for use in investigations.

We don't need to go as far as ISO 27001 but some of the controls are useful (Taken from ISO 27001 A.10.10).

**Audit logging**&#x20;

Audit logs recording user activities, exceptions, and information security events shall be produced and kept for an agreed period to assist in future investigations and access control monitoring.

**Monitoring system use**&#x20;

Procedures for monitoring the use of information processing facilities shall be established, and the results of the monitoring activities reviewed regularly.&#x20;

**Protection of log information**&#x20;

Logging facilities and log information shall be protected against tampering and unauthorized access.&#x20;

**Administrator and operator logs**&#x20;

System administrator and system operator activities shall be logged.&#x20;

**Fault logging**&#x20;

Faults shall be logged, analyzed, and appropriate action taken.

## Why do Logs Matter for Security and Compliance? <a href="#template-auditlogs-whydologsmatterforsecurityandcompliance" id="template-auditlogs-whydologsmatterforsecurityandcompliance"></a>

Without sufficient collection, regular review and long-term retention of logs, your organization will not be in compliance with regulations nor able to protect its information assets properly. Logs provide a way to monitor your systems and keep a record of security events, information access and user activities. In some cases, event logging may have to be barred because of privacy reasons.

### Event Logging <a href="#template-auditlogs-eventlogging" id="template-auditlogs-eventlogging"></a>

Control- Event logs should be produced, retained, and regularly reviewed to record user activities, exceptions, defects, and information security events.

Implementation Guidance- Where applicable, event logs should include:

1. IDs of User
2. Activities of the system: dates, times and key events details, such as log-on and log-off
3. System ID or location and device recognition, where possible, records of the attempts to access the system successfully, as well as rejected ones successful and unsuccessful data records and other attempts to access resources system configuration alterations, utilization of privileges, the application and use of systems utilities
4. Accessed files and access kinds: network addresses and protocols
5. Entry management system warnings
6. Protective mechanisms such as anti-virus and intrusion detection systems are activated and deactivated as required
7. Transaction records are done in applications by users.

\
