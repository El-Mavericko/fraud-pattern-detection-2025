# fraud-pattern-detection-2025  
**Fraud patterns detected and neutralized.**

## Synthetic ID Fraud Detection – Teleco Case Study

### Overview  
This repo documents an observed fraud pattern at the point of customer sign-up within the telecoms space, based on my experience as a Fraud Operations Analyst in UK telecommunications. The behavior is consistent with coordinated synthetic ID fraud involving subtle identity mutations and template reuse.

The purpose of this documentation is to:
- Break down the fraud behaviour observed  
- Highlight limitations in current detection systems  
- Explore the alignment with IPQS technology  
- Propose a lightweight pilot framework to test effectiveness  

---

## 1. Fraud Pattern Summary

- **Attack Vector:** Customer sign-up / credit application  
- **Technique:** Use of authentic ID templates with slight name or photo alterations  
- **Signature Behavior:** Repetitive use of the same document layout, address details, or data structure with minor mutations (e.g., “Maddy” → “Meddy”)  
- **Location Bias:** Repeated orders to specific delivery locations and sign-ups placed under different accounts with overlapping IP activity  

---

## 2. System Weaknesses Identified

- No real-time flagging of name inconsistencies  
- Lack of email string validation or historical risk scoring  
- No device/IP cross-referencing at the sign-up stage  
- Manual review only identifies fraud after escalation  

---

## 3. Proposed Solution – IPQS Alignment

**Vendor:** IPQS (Fraud and cyber threat intelligence platform)

**Relevant Capabilities:**
- **Email string risk scoring:** Detects fake, newly created, or bot-generated emails  
- **Device fingerprinting:** Flags reuse of devices across multiple sign-ups  
- **IP reputation scoring:** Identifies VPN/proxy usage and known fraud infrastructure  
- **Real-time scoring engine:** Analyzes behavior and metadata at the point of entry  

---

## 4. Pilot Concept – VMO2 Simulation

**Objective:**  
Run IPQS scoring in parallel with VMO2’s current sign-up process for 30 days  

**Inputs:**  
Anonymized customer sign-up metadata  

**Outputs:**  
Comparison between IPQS detections and internal fraud flags  

**Evaluation Metrics:**  
Detection rate, anomaly speed, overlap with known fraudsters, false positives  

---

## 5. Personal Note

This repo is part of a broader mission to modernize and enhance fraud prevention in high-volume, high-risk customer onboarding environments — by leveraging frontline intelligence and strategic technologies.

*Created by: Michael Kolawole*  
*Fraud Operations Analyst | Aspiring Cybersecurity Strategist*
