# Compliance Framework: PCI-DSS v4.0
## Clause / Identifier: Requirement 3.4

> ℹ️ **COMPLIANCE CHUNK**
> *This is an atomic unit of a larger compliance framework. It is designed to be easily referenced by Agentic Skills, Recipes, and Project Requirements.*

## 📜 Core Requirement Text
Render PAN (Primary Account Number) unreadable anywhere it is stored (including on portable digital media, backup media, and in logs) by using any of the following approaches: 
- One-way hashes based on strong cryptography
- Truncation (hashing cannot be used to replace the truncated segment of PAN)
- Index tokens and pads (pads must be securely stored)
- Strong cryptography with associated key-management processes and procedures.

## 🎯 Applicability Criteria
- **Triggers:** Any feature, database schema change, or log stream modification that could potentially capture or store a 15-to-19 digit account number used for payment.
- **Exemptions:** Systems that only handle post-authorization transaction IDs or pre-tokenized values provided by approved external gateways.

## 🔗 Related Internal Resources
- **Required Recipes:** `../recipes/payment_processing_recipe.md`
- **Responsible Department:** Security Compliance

---
**Governance Metadata**
- **Framework Version:** PCI-DSS v4.0
- **Last Validated:** 2024-05-20
