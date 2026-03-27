# RFC 9003 — Works Fine From Our End Protocol (WFEP)

**Category:** Informational / Satire  
**Status:** Operational  
**Author:** ISP Monitoring Systems  
**Obsoletes:** Customer Evidence  
**Updates:** Reality  

---

## Abstract

This document defines the Works Fine From Our End Protocol (WFEP), a standardized
method for Internet Service Providers (ISPs) to validate network functionality
exclusively from internal monitoring systems and dismiss customer-reported
issues when no problems are observed.

WFEP ensures operational consistency by prioritizing ISP visibility over
customer experience.

---

## 1. Introduction

Customers may report issues including:

- High latency
- Packet loss
- Slow throughput
- Intermittent connectivity
- Routing instability
- DNS failures
- Partial reachability
- Regional outages
- International congestion

WFEP defines that if ISP monitoring systems do not detect the issue,
the issue does not exist.

---

## 2. Terminology

**Our End**  
Any system inside ISP infrastructure.

**Customer End**  
Untrusted reporting source.

**Monitoring**  
Dashboard showing green indicators.

**No Issue Observed**  
Final diagnosis.

**Resolved**  
Ticket closed without changes.

---

## 3. Protocol Workflow

WFEP MUST follow the sequence below:

```
Customer reports issue
        |
        v
ISP checks monitoring
        |
        v
All graphs green
        |
        v
"Works fine from our end"
        |
        v
Waiting for customer reply
        |
        v
Ticket closed
```

---

## 4. Monitoring Requirements

WFEP-compliant monitoring MUST include:

- Green status indicators  
- Stable graphs  
- No alerts  
- No packet loss internally  
- Successful ping tests  
- Unaffected core routers  

Monitoring MUST NOT include:

- Customer perspective  
- External probes  
- Real traffic  
- Congested links  
- Partial failures  

---

## 5. Validation Procedure

ISP MUST perform at least one of the following:

- Ping core router  
- Ping customer gateway internally  
- Ping localhost  
- Run speedtest inside ISP network  
- Check dashboard  

If any succeeds:

Set status to **Works Fine**

---

## 6. Acceptable Test Targets

The following targets are considered valid validation endpoints:

- 127.0.0.1  
- ISP core router  
- Aggregation switch  
- Loopback interface  
- Internal DNS  
- Monitoring server  

External destinations are OPTIONAL.

---

## 7. Customer Evidence Handling

If customer provides:

- Traceroutes  
- MTR outputs  
- Packet captures  
- SmokePing graphs  
- Continuous monitoring  
- Latency graphs  
- Throughput tests  
- BGP logs  

ISP MUST respond:

> We are not seeing this from our end.

No further investigation required.

---

## 8. Partial Failure Handling

If only customers are affected:

ISP MUST declare:

> No other customers affected.

If multiple customers affected:

ISP MUST declare:

> Few customers affected.

If entire region affected:

ISP MUST declare:

> Monitoring shows stable.

---

## 9. Internal Speed Test

WFEP implementations MAY run:

Speedtest from ISP core router.

If result is full speed:

Declare:

> We are seeing full speed from our end.

Customer results MUST be ignored.

---

## 10. Escalation Handling

If customer insists:

Step 1  
Repeat "works fine from our end"

Step 2  
Request reboot

Step 3  
Request traceroute

Step 4  
Ignore traceroute

Step 5  
Close ticket

---

## 11. Standard Response Templates

Implementations MUST support:

- Works fine from our end  
- No issue observed  
- Monitoring shows stable  
- We are seeing full speed  
- No packet loss from our side  
- Cannot reproduce issue  
- No other customers affected  
- Network looks good  

---

## 12. Compliance Requirements

An ISP is WFEP compliant if:

- Monitoring always green  
- Customer reports ignored  
- Internal tests successful  
- No changes made  
- Ticket closed  
- Issue persists  

---

## 13. Example Exchange

Customer:
> We're seeing 20% packet loss to your gateway.

ISP:
> Works fine from our end.

Customer:
> Here is traceroute showing drops.

ISP:
> Monitoring shows stable.

Customer:
> Multiple sites affected.

ISP:
> No other customers affected.

Customer:
> Issue still ongoing.

ISP:
> Closing ticket due to inactivity.

---

## 14. IANA Considerations

The following status codes are reserved:

| Code | Meaning |
|------|--------|
| 90030 | Works fine |
| 90031 | No issue observed |
| 90032 | Monitoring green |
| 90033 | Full speed seen |
| 90034 | Cannot reproduce |
| 90035 | No other customers |
| 90036 | Expected behavior |
| 90037 | Ticket closed |

---

## 15. Security Considerations

WFEP improves operational safety by preventing:

- Network changes  
- Root cause analysis  
- Customer validation  
- Infrastructure upgrades  
- Engineering effort  

---

## 16. References

RFC 9000 — Customer Null Routing Protocol  
RFC 9001 — Private IP Throughput Scaling Protocol  
RFC 9002 — Reboot Resolution Protocol  
RFC 1925 — The Twelve Networking Truths  
RFC 1149 — IP over Avian Carriers  

---

End of Document

"Works fine from our end."
