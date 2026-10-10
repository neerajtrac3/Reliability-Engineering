
# 🔍 Change‑Point Detection

Change‑Point Detection is a statistical technique used to identify **sudden shifts** in system behavior, failure patterns, or reliability trends. In reliability engineering, detecting these shifts early is critical for preventing outages, reducing downtime, and improving operational stability — especially in mission‑critical systems such as banking, payments, cloud infrastructure, and distributed microservices.

---

## 📌 Why Change‑Point Detection Matters

Change‑points often indicate:

- A sudden increase in failure rate  
- A degradation in system reliability  
- A new workload pattern  
- A configuration or deployment issue  
- A hidden fault propagating through the system  
- A shift in user behavior or transaction volume  

Detecting these changes early allows engineers to:

- Trigger preventive maintenance  
- Adjust capacity or scaling  
- Investigate anomalies  
- Improve SLM reliability scoring  
- Prevent cascading failures  

---

## 📊 Types of Change‑Points

### **1. Mean Shift**
A sudden jump in average failure time or error count.

### **2. Variance Shift**
System becomes more unstable or unpredictable.

### **3. Trend Shift**
Failure rate begins increasing or decreasing sharply.

### **4. Distribution Shift**
Underlying statistical behavior changes (e.g., new failure mode).

---

## 🧮 Common Change‑Point Detection Methods

### **1. CUSUM (Cumulative Sum Control Chart)**  
Detects small but persistent shifts.

```text
S(t) = max(0, S(t-1) + (x(t) - k))
Change detected when S(t) > h
```

Where:  
- **k** = reference value  
- **h** = threshold  

---

### **2. Moving Average / Rolling Window**
Compares short‑term vs long‑term averages.

```text
Change detected when:
ShortTermAvg - LongTermAvg > Threshold
```

---

### **3. Bayesian Change‑Point Detection**
Probabilistic method for detecting structural changes.

Used when failures follow non‑stationary patterns.

---

### **4. Statistical Tests**
- t‑test  
- Kolmogorov–Smirnov test  
- Likelihood ratio tests  

Used to detect distribution shifts.

---

## 🧩 Illustrative Example (Conceptual)

```text
Failure times:
[10, 12, 13, 15, 40, 42, 45]

Observation:
Sudden jump from ~15 to ~40 indicates a change‑point.

Interpretation:
System reliability degraded sharply.
```

This kind of jump often signals:

- A new failure mode  
- A configuration change  
- A workload spike  
- A hidden defect emerging  

---

## 🏦 Industry Use Cases

Change‑point detection is essential for:

- Payment switch anomaly detection  
- ATM network reliability monitoring  
- Fraud detection pipeline stability  
- Core banking batch performance  
- Cloud datacenter reliability  
- Microservices error‑rate monitoring  
- Legacy TPF/ALCS degradation tracking  

It directly feeds into **SLM reliability scoring**, **failure rate analysis**, and **AI‑based forecasting**.

---

## 🔗 Related Sections

- Reliability Growth Modeling  
- Failure Rate & Hazard Analysis  
- MTBF / MTTR  
- SLM Reliability Score  

---

