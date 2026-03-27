# RFC 9004 — Integrated ONT Throughput Limitation Protocol (IOTLP)

**Category:** Informational / Satire  
**Status:** WiFi Connected  
**Author:** ISP CPE Deployment Team  
**Obsoletes:** End-to-End Throughput  
**Updates:** Customer Expectations  

---

## Abstract

This document defines the Integrated ONT Throughput Limitation Protocol (IOTLP),
a standardized deployment model where ISPs provide integrated ONT devices with
built-in WiFi and LAN ports while provisioning gigabit service plans that cannot
be practically achieved using the provided equipment.

IOTLP ensures customers subscribe to high-speed plans while experiencing
significantly lower throughput over default connectivity methods.

---

## 1. Introduction

ISPs increasingly deploy integrated ONT devices that include:

- Built-in WiFi
- 4 LAN ports
- Single power adapter
- Default SSID
- Admin access disabled
- Unknown chipset
- 100 Mbps real-world WiFi throughput

Customers are provisioned with:

- 500 Mbps plans
- 1 Gbps plans
- "Ultra Fiber" branding
- "Lightning Speed" marketing

IOTLP defines that full speed is only achievable via wired connection.

---

## 2. Terminology

**Integrated ONT**  
Single device combining ONT, router, WiFi, and limitations.

**WiFi Speed**  
Theoretical number printed on box.

**LAN Speed**  
Speed achievable only with customer-provided cable.

**Customer Responsibility**  
Anything not included by ISP.

**Full Speed**  
Available but inaccessible.

---

## 3. Deployment Model

ISP MUST deploy:

```
Fiber → ONT with WiFi → Customer tests over WiFi → Low speed
```

Customer MUST then be instructed:

> Please use LAN cable for full speed.

---

## 4. WiFi Throughput Behavior

The integrated ONT WiFi MUST provide:

| Plan Speed | WiFi Speed |
|------------|-----------|
| 100 Mbps | 60 Mbps |
| 300 Mbps | 95 Mbps |
| 500 Mbps | 100 Mbps |
| 1 Gbps | 100 Mbps |

ISP MUST declare:

> WiFi speed depends on environment.

---

## 5. LAN Speed Requirement

Full speed MUST require:

- Gigabit Ethernet
- Proper cable
- Short distance
- Compatible device
- Customer effort

ISP MUST NOT provide cable.

---

## 6. Cable Responsibility Transfer

Customer:
> Can you provide LAN cable?

ISP:
> Not in our scope.

Customer:
> How do I test 1 Gbps?

ISP:
> Please arrange cable.

Customer:
> You installed device.

ISP:
> Cable not included.

Ticket resolved.

---

## 7. Default Installation Procedure

Technician MUST:

1. Install ONT  
2. Connect fiber  
3. Enable WiFi  
4. Run speedtest on phone  
5. Observe 80 Mbps  
6. Declare working  

No LAN test required.

---

## 8. Advanced Troubleshooting

If customer reports low speed:

ISP MUST perform:

Step 1  
Ask connection type

Step 2  
If WiFi  
Blame WiFi

Step 3  
Ask to use LAN

Step 4  
Do not provide cable

Step 5  
Close ticket

---

## 9. Gigabit Plan Validation

To validate gigabit plan, ISP MAY:

- Run speedtest from ONT internally  
- Run speedtest from technician laptop (with hidden cable)  
- Show screenshot  
- Disconnect cable  

Customer MUST not see cable.

---

## 10. Compliance Requirements

An ISP is IOTLP compliant if:

- Gigabit plan sold  
- WiFi limited to ~100 Mbps  
- Cable not provided  
- Customer asked to arrange cable  
- Full speed never demonstrated  
- Ticket closed  

---

## 11. Example Exchange

Customer:
> I'm on 1 Gbps plan but getting 90 Mbps.

ISP:
> Are you using WiFi?

Customer:
> Yes.

ISP:
> Please use LAN cable.

Customer:
> Did you provide one?

ISP:
> Not in our scope.

Customer:
> How do I test?

ISP:
> Arrange cable and check.

Ticket closed.

---

## 12. IANA Considerations

The following speeds are reserved:

| Speed | Meaning |
|-------|--------|
| 90 Mbps | WiFi normal |
| 95 Mbps | Best effort |
| 100 Mbps | Maximum WiFi |
| 1 Gbps | Marketing |
| Full Speed | Cable required |

---

## 13. Security Considerations

IOTLP improves operational safety by preventing:

- Customers verifying gigabit speed  
- Proper throughput validation  
- WiFi upgrades  
- Better CPE deployment  
- Accountability  

---

## 14. References

RFC 9000 — Customer Null Routing Protocol  
RFC 9001 — Private IP Throughput Scaling Protocol  
RFC 9002 — Reboot Resolution Protocol  
RFC 9003 — Works Fine From Our End Protocol  
RFC 1925 — The Twelve Networking Truths  

---

End of Document

"Please use LAN cable for full speed."
