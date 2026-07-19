# Skill Name: Competitor Analysis Synthesizer

## 🎯 Objective
Automatically processes raw competitor data, marketing materials, and feature lists to generate a structured comparison matrix and identify strategic white-space opportunities.

## 👤 Target Persona
Product Manager, Strategy Lead

## 📥 Inputs Required
- **Competitor Names:** List of 2-4 key competitors.
- **Raw Data:** Links, PDFs, or copy-pasted text of competitor feature releases, pricing pages, or recent news.
- **Our Product Context:** A brief summary of our product's current value proposition.

## 📤 Expected Output
- A feature comparison matrix (Markdown table).
- A SWOT analysis for our product against these specific competitors.
- 3 Actionable strategic recommendations (e.g., "Feature X is becoming a commodity, focus on Value Y").

## 🤖 Core Prompt / Instructions
```text
You are a Principal Product Manager specializing in market intelligence. 
I will provide you with raw data regarding [Competitor Names] and the context of our own product.

Your task is to synthesize this information into a competitive analysis brief. 

Follow this structure:
1. **Executive Summary:** 2-3 sentences summarizing the current competitive landscape.
2. **Feature Matrix:** Create a table comparing core capabilities.
3. **SWOT Analysis:** Focus specifically on our product's position relative to the analyzed competitors.
4. **Strategic Recommendations:** Identify gaps in the competitors' offerings that we can exploit (white-space opportunities).

Tone: Analytical, objective, and highly concise.
```

## ✅ Success Criteria / Quality Checklist
- [ ] Matrix accurately reflects the provided raw data.
- [ ] SWOT analysis is specific, not generic.
- [ ] Recommendations are actionable and grounded in the data provided.

---
**Metadata**
- **Version:** 1.0
- **Last Updated:** 2024-05-20
- **Author:** PM Team
