
# ⏱️ MTBF / MTTR Calculations

**MTBF (Mean Time Between Failures)** and **MTTR (Mean Time To Repair)** are foundational reliability engineering metrics. They help quantify system availability, stability, and maintainability — especially in mission‑critical environments such as banking, payments, cloud infrastructure, and distributed systems.

These metrics form the basis of **availability calculations**, **SLM reliability scoring**, and **failure forecasting**.

---

## 📌 MTBF — Mean Time Between Failures

MTBF measures the average operating time between two consecutive failures.

### **Formula**
```text
MTBF = Total Operating Time / Number of Failures
```

### **Interpretation**
- Higher MTBF → system runs longer without failing  
- Lower MTBF → failures occur frequently  
- Used for: uptime planning, maintenance scheduling, reliability scoring  

---

## 📌 MTTR — Mean Time To Repair

MTTR measures how long it takes to restore a system after a failure.

### **Formula**
```text
MTTR = Total Repair Time / Number of Repairs
```

### **Interpretation**
- Lower MTTR → faster recovery  
- Higher MTTR → slow repair cycles, poor maintainability  
- Used for: SLA planning, incident response, operational readiness  

---

## 📈 Availability Calculation

MTBF and MTTR together determine system availability.

### **Formula**
```text
Availability = MTBF / (MTBF + MTTR)
```

### **Meaning**
- Availability approaches **1.0** when MTBF ≫ MTTR  
- Availability drops when MTTR increases or MTBF decreases  

---

## 🧩 Example (Conceptual)

```text
Given:
Total operating time = 1000 hours
Number of failures = 5
Total repair time = 12 hours
Number of repairs = 5

MTBF = 1000 / 5 = 200 hours
MTTR = 12 / 5 = 2.4 hours

Availability = 200 / (200 + 2.4)
Availability ≈ 0.988 (98.8%)
```

This means the system is available **98.8%** of the time.

---

## 🏦 Industry Use Cases

MTBF and MTTR are critical for:

- Payment switch uptime  
- ATM network reliability  
- Core banking batch systems  
- Fraud detection pipelines  
- Cloud datacenter operations  
- Microservices and distributed systems  
- Legacy TPF/ALCS reliability planning  

They directly feed into **SLM reliability scoring**, **change‑point detection**, and **failure rate analysis**.

---

## 🔗 Related Sections

- Failure Rate & Hazard Analysis  
- Reliability Growth Modeling  
- Change‑Point Detection  
- SLM Reliability Score  

---
