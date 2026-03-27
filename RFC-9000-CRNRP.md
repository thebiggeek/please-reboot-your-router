# RFC 9000 — Customer Null Routing Protocol (CNRP)

Category: Informational / Satire  
Status: Works Fine From Our End  
Author: ISP Support Engineering  
Obsoletes: Customer Expectations  
Updates: Nothing  

---

## Abstract

This document defines the Customer Null Routing Protocol (CNRP), a standardized
method for Internet Service Providers (ISPs) to receive, acknowledge, process,
and ultimately ignore customer requests in a scalable and operationally safe
manner.

CNRP ensures network stability by minimizing unnecessary troubleshooting,
configuration changes, and customer satisfaction.

---

## 1. Introduction

ISPs frequently receive customer requests including, but not limited to:

- "We're seeing packet loss"
- "Latency increased significantly"
- "BGP session keeps flapping"
- "Your upstream is congested"
- "Can I get a public IPv4?"
- "Your DNS resolvers are down"
- "Traffic shaping after peak hours"
- "Your gateway is dropping packets"

Such requests may require action. To prevent this, CNRP MUST be implemented.

---

## 2. Terminology

**Customer**  
An external alerting system generating tickets.

**Ticket**  
A structured container for delaying resolution.

**Engineer**  
A template-based response mechanism.

**Investigation**  
Running a single ping to a well-known IP address.

**Resolved**  
Ticket closed without making any changes.

**Monitoring**  
A dashboard permanently showing green indicators.

---

## 3. Protocol Workflow

The CNRP workflow MUST follow the sequence below:

+---------------------+
| Customer Complaint |
+----------+----------+
|
v
+---------------------+
| Ticket Created |
+----------+----------+
|
v
+---------------------+
| Auto Acknowledgement|
+----------+----------+
|
v
+---------------------+
| "No issue observed" |
+----------+----------+
|
v
+---------------------+
| Waiting for Customer|
+----------+----------+
|
v
+---------------------+
| Auto Close (48 hrs) |
+---------------------+


This workflow MUST be followed for all tickets regardless of severity.

---

## 4. Standard Response Messages

Implementations MUST support at least one of the following:

- Works fine from our end
- Please reboot your router
- No other customers affected
- Issue not reproducible
- Monitoring shows no issue
- This is expected behavior
- Please check your LAN cable
- Closing ticket due to inactivity

Advanced deployments MAY include:

- Upstream provider issue
- Maintenance window in progress
- Fiber cut (no ETA)
- Please flush DNS cache
- Try another device
- Configuration not supported

---

## 5. Investigation Procedure

Upon receiving a ticket, the ISP MUST perform:

ping 8.8.8.8 -c 1

If the ping succeeds:

set_status("Resolved")

If the ping fails:

blame_customer()
set_status("Resolved")


No further troubleshooting is required.

---

## 6. Escalation Handling

If the customer provides any of the following:

- MTR output
- Traceroutes
- Packet captures
- BGP logs
- SmokePing graphs
- Latency monitoring
- Continuous packet loss data

The ticket MUST be escalated to Tier 2.

Tier 2 MUST perform:

-------------
Close Ticket
------------

## 7. CGNAT Handling

If a customer requests a public IPv4 address, the ISP MUST respond:

> Due to IPv4 exhaustion we cannot provide public IPv4 addresses.

The ISP MAY continue allocating addresses from 100.64.0.0/10.

---

## 8. Priority Mapping

| Customer Severity | ISP Severity |
|-------------------|-------------|
| Critical          | Low         |
| High              | Low         |
| Medium            | Low         |
| Low               | Auto Close  |

---

## 9. Service Level Agreement

CNRP-compliant implementations MUST meet:

- First Response Time: < 5 minutes (automated)
- Investigation: Not required
- Resolution: Ticket closed
- MTTR: Artificially improved
- RCA: Not provided

---

## 10. Compliance Requirements

An ISP is considered CNRP compliant if:

- Tickets are acknowledged but not fixed
- Customers are asked to reboot equipment
- Monitoring always shows green
- Escalations disappear
- Issues reoccur weekly
- No configuration changes are made

---

## 11. Example Exchange

Customer:
> We see 25% packet loss to your gateway.

ISP:
> Please reboot your router.

Customer:
> This happens across multiple sites.

ISP:
> Monitoring shows no issues.

Customer:
> Here is MTR output.

ISP:
> Closing ticket due to inactivity.

---

## 12. IANA Considerations

The following ports are reserved:

| Port | Service |
|------|---------|
| 65000 | Auto Close |
| 65001 | Blame Customer |
| 65002 | Reboot Router |
| 65003 | No Issue Found |
| 65004 | Upstream Issue |
| 65005 | Expected Behavior |

---

## 13. Security Considerations

CNRP improves operational safety by preventing:

- Network changes
- Root cause analysis
- Accountability
- Customer satisfaction
- Engineering effort

---

## 14. References

RFC 1925 — The Twelve Networking Truths  
RFC 4638 — PPPoE MTU  
RFC 1149 — IP over Avian Carriers  
RFC 9000 — This Document  

---

End of Document

"Works fine from our end."


