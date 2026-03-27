# RFC 9007 — Maintenance Window Retroactive Notification Protocol (MWRNP)

**Category:** Informational / Satire  
**Status:** Completed Successfully  
**Author:** ISP Operations  
**Obsoletes:** Prior Notification  
**Updates:** Outage Messaging  

---

## Abstract

This document defines the Maintenance Window Retroactive Notification Protocol
(MWRNP), a standardized procedure for declaring outages as planned maintenance
after service restoration.

---

## 1. Introduction

Customers experience:

- Internet down
- No connectivity
- High latency
- Packet drops
- BGP reset
- Fiber outage

After recovery, ISP MUST declare maintenance.

---

## 2. Protocol Workflow

```
Network outage occurs
        |
        v
Customers complain
        |
        v
ISP silent
        |
        v
Service restored
        |
        v
"Planned maintenance"
```

---

## 3. Notification Timing

| Event | Notification |
|------|--------------|
| Before outage | None |
| During outage | None |
| After recovery | Yes |

---

## 4. Standard Messages

- Planned maintenance
- Service improvement
- Network upgrade
- Emergency maintenance
- Optimization activity

---

## 5. SLA Handling

Customer requests credit.

ISP MUST respond:

> Planned maintenance not eligible.

---

## 6. Compliance Requirements

- No prior notice  
- Outage occurs  
- Maintenance declared after  
- No credit  
- Ticket closed  

---

## Example

Customer:
> Internet was down 2 hours.

ISP:
> Planned maintenance completed.

Customer:
> No notification.

ISP:
> Emergency upgrade.

Ticket closed.

---

End of Document

"Maintenance completed successfully."
