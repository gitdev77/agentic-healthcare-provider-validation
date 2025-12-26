# Agentic AI System for Healthcare Provider Data Validation

This project implements an **agentic AI-driven data validation system** designed to improve the accuracy of healthcare provider directories by validating information across **government registries, trusted public web sources, and credential documents**.

The system dynamically adjusts confidence scores and escalates uncertain cases for human review instead of blindly automating decisions.

---

## 🚨 Problem Statement

Healthcare payers face significant challenges maintaining accurate provider directories. Studies show that **40–80% of provider records contain errors**, leading to:
- Failed appointment attempts
- Member dissatisfaction
- Regulatory risk
- High manual verification costs

Traditional systems rely heavily on **manual checks** or **single data sources**, which are slow, expensive, and error-prone.

---

## ❌ Why Existing Systems Fail

- Government registries can be outdated or incomplete  
- Public web data is dynamic but unreliable alone  
- Credential documents are unstructured and difficult to process  
- Most systems lack explainability and safe escalation mechanisms  

---

## ✅ Solution Overview

This project demonstrates a **multi-source validation pipeline** that:
1. Verifies provider identity using government registries (CMS / NPI)
2. Cross-checks official data with trusted public web sources
3. Extracts credential validity from unstructured PDF documents
4. Produces **explainable confidence scores**
5. Escalates high-risk cases for human review

---

## 🧠 System Architecture

1. **Input Provider Record**
2. **Phase 1 – Government Validation**
   - CMS NPPES (NPI) Registry API
3. **Phase 2 – Web Cross Verification**
   - Trusted healthcare websites
4. **Phase 3 – Document Intelligence**
   - PDF credential ingestion and expiry extraction
5. **Decision Engine**
   - ConfidenceScore
   - ReviewStatus:
     - AUTO-VERIFIED
     - NEEDS HUMAN REVIEW
     - CRITICAL – HUMAN REVIEW

---

## 🛠 Tech Stack

- Python
- Pandas
- Requests
- BeautifulSoup
- pdfplumber
- Regular Expressions
- CMS NPPES API

---

## 📊 Key Features

- Multi-source data validation
- Ethical web scraping with anti-bot handling
- Document-based credential verification
- Explainable confidence scoring
- Human-in-the-loop escalation logic

---

## 📈 Impact

- Reduces manual provider verification effort
- Improves directory accuracy
- Prevents unsafe automation
- Aligns with real healthcare compliance workflows

---

## 🔮 Future Enhancements

- Batch document ingestion
- OCR for scanned PDFs
- Analytics dashboard
- Workflow automation integration

---

## 🧾 Development Notes

This project was built iteratively with a focus on **decision safety, explainability, and real-world constraints** such as incomplete and conflicting data. Modern AI tools were used to accelerate development, while all validation logic and confidence scoring decisions were intentionally designed to reflect enterprise healthcare workflows.

---

## 📸 Sample Output

See the `screenshots/` folder for example outputs.
