# RFC 9009 — Speedtest Server Selection Manipulation Protocol (SSSMP)

**Category:** Informational / Satire  
**Status:** Full Speed  
**Author:** ISP NOC  
**Obsoletes:** Real Testing  
**Updates:** Speed Validation  

---

## Abstract

This document defines the Speedtest Server Selection Manipulation Protocol
(SSSMP), where ISPs instruct customers to use ISP-hosted speedtest servers
to demonstrate full bandwidth.

---

## 1. Introduction

Customer reports slow speed.

ISP instructs:

> Use our speedtest server.

---

## 2. Testing Model

```
Customer slow internet
        |
        v
ISP speedtest server
        |
        v
Full speed
        |
        v
Ticket closed
```

---

## 3. Valid Servers

- ISP hosted server  
- Same POP server  
- Internal network  
- Same rack  

External servers invalid.

---

## 4. Standard Response

> We see full speed on our server.

---

## 5. Compliance Requirements

- Internal test only  
- Full speed shown  
- External slow ignored  
- Ticket closed  

---

## Example

Customer:
> Getting 200 Mbps.

ISP:
> Test using our server.

Customer:
> Now 1 Gbps.

ISP:
> Line working fine.

Ticket closed.

---

End of Document

"Use our speedtest server."
