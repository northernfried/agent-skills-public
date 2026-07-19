# Compliance Framework: [e.g., PCI-DSS, GDPR, HIPAA]

## Clause / Identifier: [e.g., Requirement 3.4, Article 32]

> ℹ️ **COMPLIANCE CHUNK**
> *This is an atomic unit of a larger compliance framework. It is designed to be easily referenced by Agentic Skills, Recipes, and Project Requirements.*

## 📜 Core Requirement Text

[Provide the exact, verbatim text of the compliance clause or a highly accurate, legally approved summary.]

> *"Render PAN unreadable anywhere it is stored (including on portable digital media, backup media, and in logs) by using any of the following approaches: One-way hashes based on strong cryptography, Truncation, Index tokens and pads, or Strong cryptography with associated key-management processes and procedures."*

## 🎯 Applicability Criteria

[Define clearly when a project or feature must trigger this compliance chunk.]

- **Triggers:** [e.g., Any feature that accepts, transmits, or stores Primary Account Numbers (PAN).]
- **Exemptions:** [e.g., Systems that only handle tokenized transaction IDs provided by a third-party payment gateway (Stripe/Adyen) where no raw PAN touches our servers.]

## 🔗 Related Internal Resources

- **Required Recipes:** [Link to the Recipes that implement this, e.g., `recipes/payment_processing_recipe.md`]
- **Responsible Department:** [e.g., InfoSec Compliance Team]

---

## Governance Metadata

- **Framework Version:** [e.g., v4.0]
- **Last Validated:** YYYY-MM-DD
