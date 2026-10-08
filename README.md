# Phising_Email_Forensic_Analyser & Link Defanger

A modular Python tool for **safe phishing email analysis, link defanging, domain spoof detection, and risk scoring**.

## Features

*  Parse `.eml` files or raw RFC 822 email text
*  Extract and **defang URLs** (`https://` → `hxxps://`)
*  Detect sender/link **domain mismatches**
*  Identify phishing-related language using NLP keyword analysis
*  Generate an explainable **0–100 risk score**
*  Interactive **Gradio dashboard**
*  Includes end-to-end self-tests

## Modules

```text
modules/
├── email_parser.py
├── link_defanger.py
├── nlp_analyzer.py
└── risk_scorer.py
```

## Risk Levels

| Score  | Risk          |
| ------ | ------------- |
| 0–34   | 🟢 Safe       |
| 35–69  | 🟡 Suspicious |
| 70–100 | 🔴 Dangerous  |

## Example Result

A simulated PayPal phishing email was detected with:

**Score:** `64/100`
**Verdict:** `SUSPICIOUS`

A benign internal email received:

**Score:** `0/100`
**Verdict:** `SAFE`

## Tech Stack

* Python
* Google Colab
* Regex
* `tldextract`
* NLP Lexicon Analysis
* Pandas
* Gradio

## Project

**Course:** CSE 4174 — Cyber Security Lab
**Group:** G107
**Department:** Computer Science & Engineering
**Ahsanullah University of Science and Technology (AUST)**
