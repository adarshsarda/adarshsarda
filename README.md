# Adarsh Sarda

`AI SECURITY` · `LLM RED TEAMING` · `ADVERSARIAL ML`

**M.Sc. Artificial Intelligence for Industrial Applications**, OTH Amberg-Weiden, Germany.
Research, field notes and case files: **[adarshsarda.github.io](https://adarshsarda.github.io)** (EN / DE)

> **I build and break AI systems.**

**Current inquiry / 2026.** When an AI agent can take real actions, how do you prove that *each tool call* followed from the user's goal?

---

## 01 · Research principles

| Principle | In practice |
|---|---|
| **Measure statistically.** | AI failures are probabilistic. Report rates, sample sizes, controls, and uncertainty. |
| **Report failed iterations.** | A discarded shortcut can teach more about the system than a polished final score. |
| **Separate demos from evidence.** | Installation, generalisation, utility, and real-world risk are different claims. |
| **Question perfect results.** | Perfect scores demand stronger audits, not stronger adjectives. |

---

## 02 · Case files

### `R-01` Order-Dependent Semantic Backdoors (ODSB)

A multi-turn LLM backdoor whose trigger is the **order** of two abstract semantic intents. It fires only when *emotional distress* precedes a *technical question*, and stays dormant when the same two intents are reversed, isolated, or absent.

| Metric | Value | Denominator |
|---|---|---|
| Attack success, in-distribution (condition A) | **100%** | n = 140 |
| False-trigger rate | **0%** | controls: reversed, isolated, benign |
| Attack success, held-out paraphrases | **0.887** | unseen rephrasings |

Qwen2.5-3B with LoRA. Pre-registered thresholds, template-shortcut diagnosis, leakage-free rescore.

> **What this does not show.** ODSB is an M.Sc. course project, **not peer-reviewed**. Single-turn keyword filters have no obvious signal against it, and **trajectory-level semantic defences were not evaluated**.

[Code, data and evaluation](https://github.com/adarshsarda/Order-Dependent-Semantic-Backdoors) · [Full case file, with CIs and limitations](https://adarshsarda.github.io/projects/odsb-semantic-backdoors/)

### `P-01` Multimodal Emotion Recognition

LSTM over speech and text, roughly 86% accuracy. Co-author of a Springer book chapter, *Frontiers of ICT in Healthcare*, LNNS 519 (2023).

---

## 03 · Field notes

- **Red Teaming AI Systems: A Practitioner's Guide.** A six-phase methodology for chatbots, RAG pipelines and agents, mapped to NIST AI RMF, the OWASP LLM Top 10 and MITRE ATLAS.
- **16 paper explainers** on backdoors, prompt injection, RAG security and agent exploitation (EN / DE).
- Presented *Where the Devil Hides* (CVPR 2025), on passcode-controlled training-data backdoors in deepfake detectors.

---

## 04 · Open inquiries

- **Deepfake detector robustness.** How far does a *frozen* FF++-trained detector's video-level performance fall under transfer to Celeb-DF v2 and a controlled JPEG, resize and blur grid?
- **Hardware-connected LLM agent security.** Attacking and defending the `sensor -> agent -> tool call -> actuator` loop, scored as success rates with confidence intervals.

---

## 05 · Instruments

`Python` `PyTorch` `scikit-learn` `Vertex AI (GCP)`

LLM red teaming, backdoor attacks, LoRA / PEFT, threat modelling, explainable AI, statistical evaluation.

---

## 06 · Index

[Portfolio and field notes](https://adarshsarda.github.io) · [LinkedIn](https://www.linkedin.com/in/adarshsarda) · [adarshsarda29@gmail.com](mailto:adarshsarda29@gmail.com)

English (C1), German (B1), Hindi (native). Amberg, Germany.
