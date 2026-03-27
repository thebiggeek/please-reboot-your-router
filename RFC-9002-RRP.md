# RFC 9002 — Reboot Resolution Protocol (RRP)

**Category:** Informational / Satire  
**Status:** Power Cycling  
**Author:** ISP Support Operations  
**Obsoletes:** Troubleshooting  
**Updates:** Customer Patience  

---

## Abstract

This document defines the Reboot Resolution Protocol (RRP), a standardized
operational procedure for resolving all network-related issues by requesting
the customer to reboot one or more devices regardless of fault domain.

RRP reduces troubleshooting complexity by replacing diagnostics with power
cycling. This ensures predictable support workflows and minimizes engineering
effort.

---

## 1. Introduction

Customers frequently report issues such as:

- Slow internet
- Packet loss
- High latency
- BGP flapping
- Fiber down
- DNS failures
- Routing loops
- Entire region outage
- Submarine cable cut
- Power failure at ISP POP

RRP defines that all such issues MUST be resolved by rebooting customer
equipment.

---

## 2. Terminology

**Reboot**  
Turning a device off and on while hoping.

**Power Cycle**  
Reboot with additional waiting time.

**Cold Reboot**  
Longer reboot for increased confidence.

**Reboot Loop**  
Successful troubleshooting process.

**Resolved**  
Customer stopped replying.

---

## 3. Protocol Workflow

RRP MUST follow the sequence below:

```
Customer Complaint
        |
        v
"Please reboot router"
        |
        v
Customer already rebooted
        |
        v
"Please reboot modem"
        |
        v
Customer already rebooted
        |
        v
"Please reboot both together"
        |
        v
Waiting 24 hours
        |
        v
Ticket Closed
```

---

## 4. Mandatory Reboot Targets

The ISP MUST request reboot of at least one of the following:

- Router  
- Modem  
- ONT  
- Switch  
- Firewall  
- Wi-Fi Access Point  
- Customer Laptop  
- Customer Phone  
- Entire Rack  
- Power Strip  
- Building Power (if accessible)

Advanced implementations MAY include:

- Restart browser  
- Restart speedtest  
- Restart Ethernet cable  
- Restart ISP  

---

## 5. Reboot Escalation Levels

| Level | Action |
|------|--------|
| L1 | Reboot router |
| L2 | Reboot modem |
| L3 | Reboot both |
| L4 | Reboot sequentially |
| L5 | Reboot simultaneously |
| L6 | Wait 5 minutes and reboot again |
| L7 | Factory reset |
| L8 | Replace working hardware |
| L9 | Close ticket |

---

## 6. Investigation Procedure

Upon receiving any complaint, ISP MUST perform:

Step 1  
Ask customer to reboot

Step 2  
If customer confirms reboot completed  
Ask customer to reboot again

Step 3  
If issue persists  
Escalate to "cold reboot"

Step 4  
Close ticket

---

## 7. Cold Reboot Requirements

Cold reboot MUST follow:

1. Power off device  
2. Wait 30 seconds  
3. Say "please wait"  
4. Wait additional 2 minutes  
5. Power on  
6. Issue still present  
7. Declare monitoring

---

## 8. Simultaneous Reboot Mode

If multiple devices exist, ISP MUST instruct:

> Please turn off modem and router at same time.

Customer confusion is REQUIRED.

---

## 9. Special Case Handling

### 9.1 Fiber Cut

Customer:
> Fiber link is physically cut

ISP:
> Please reboot router

---

### 9.2 BGP Session Down

Customer:
> BGP neighbor down

ISP:
> Please restart router

---

### 9.3 Regional Outage

Customer:
> Entire city down

ISP:
> Please reboot modem

---

### 9.4 Submarine Cable Failure

Customer:
> International latency high

ISP:
> Please reboot and check

---

## 10. Auto Close Behavior

If customer does not respond after reboot request:

Ticket MUST be closed with:

> Issue resolved after reboot.

---

## 11. Standard Response Templates

Implementations MUST support:

- Please reboot your router
- Please reboot modem and router
- Please power cycle device
- Turn off and on again
- Reboot and check
- Try after restart
- Restart both devices
- Cold reboot required

---

## 12. Compliance Requirements

An ISP is RRP compliant if:

- Every ticket includes reboot request  
- Diagnostics not performed  
- Multiple reboots requested  
- Issue unchanged  
- Ticket closed  
- Customer exhausted  

---

## 13. Example Exchange

Customer:
> We're seeing packet loss to your gateway.

ISP:
> Please reboot router.

Customer:
> This is a dedicated link.

ISP:
> Please reboot modem.

Customer:
> This is fiber handoff.

ISP:
> Please reboot both.

Customer:
> This is upstream congestion.

ISP:
> Monitoring now.

Ticket closed.

---

## 14. IANA Considerations

The following reboot codes are reserved:

| Code | Meaning |
|------|--------|
| 9002 | Reboot router |
| 9003 | Reboot modem |
| 9004 | Reboot both |
| 9005 | Cold reboot |
| 9006 | Reboot again |
| 9007 | Factory reset |
| 9008 | Ticket closed |

---

## 15. Security Considerations

RRP improves operational safety by preventing:

- Root cause analysis  
- Network changes  
- Engineer involvement  
- Accountability  
- Fixing the issue  

---

## 16. References

RFC 9000 — Customer Null Routing Protocol  
RFC 9001 — Private IP Throughput Scaling Protocol  
RFC 1925 — The Twelve Networking Truths  
RFC 1149 — IP over Avian Carriers  

---

End of Document

"Please reboot and confirm."
