# NeoNurture 🍼

NeoNurture is an early-stage AI platform that applies clinician-supervised NLP and information-structuring workflows delivered as a secure cloud-based system (rather than a monolithic legacy EMR architecture - Cache, MUMPS, etc.) designed for clinical environments, with the goal of improving continuity-of-care and family-centered communication throughout the NICU course and discharge transition.

> Status: dev/field research + prototyping only. Not for clinical use [yet :)].

---

## What We're Exploring

🔍 **LLM-assisted clinical information extraction**: NICU-style free-text notes segmented and normalized, and key entities (respiratory support, nutrition, growth metrics, clinical events, etc.) are mapped into a structured, typed schema using constrained LLM workflows.

🧾 **Schema-conditioned natural-language [NLP] generation for families**: Family-readable summaries generated from said structured representation, not raw notes, to preserve grounding and auditability. Prompts enforce restatement-only constraints, excluding medical advice, interpretation, or prognosis.

⏱️ **Longitudinal narrative synthesis**: Entries are time-aligned across encounters so changes are represented as a coherent narrative, supporting continuity during NICU-to-pediatrics transitions.

🛡️ **Embedded guardrails and human-in-the-loop review**: Task-scoping limits prohibit diagnosis, treatment recommendation, risk scoring, or independent interpretation. All official outputs will require clinician review.

> All work is currently done on **synthetic or de-identified data**. Any real-world deployment will require appropriate IRB.

---

## Current Prototype

🔬 **LLM Translator Prototype:**  
A minimal working pipeline that:
- ingests "chart" notes
- extracts key clinical fields into a structured framework using supervised LLM prompting
- generates restatement-only family-readable draft from delineation for clinician review

This prototype is limited to controlled test notes and does not perform diagnosis, risk scoring, or treatment recommendation.
  Repo: [`neonurture-llm-translator`](https://github.com/giakerney/neonurture_llm_translator)
  
---

## Contact

If you’re interested in neonatal medicine, AI in healthcare, or want to help expand NeoNurture, feel free to reach out!
