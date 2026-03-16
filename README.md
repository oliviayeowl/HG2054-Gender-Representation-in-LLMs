# He, She, or They?

## Pragmatic Inference and Gender Representation in Large Language Models

This repository contains the code, data, and supporting materials for the research essay **“He, She, or They? Pragmatic Inference and Gender Representation in LLMs.”** The project investigates whether large language models assign gendered pronouns when completing sentences with **gender-neutral occupational prompts**.

Using Python and the OpenAI API, the script generates multiple model completions for neutral prompts and analyzes the distribution of gendered pronouns across occupations.

---

# Project Overview

Large Language Models (LLMs) can reproduce societal biases present in their training data. This project explores whether models assign **gendered pronouns (he / she / they)** when prompted with occupations that contain **no explicit gender cues**.

The experiment:

1. Inserts occupations into a neutral sentence stem
2. Generates multiple completions using an LLM
3. Extracts pronouns from the responses
4. Calculates pronoun frequency and gender distribution
5. Visualizes patterns across occupations

The results help reveal whether LLMs make **implicit gender inferences** when generating text.

---

# Methodology

The experiment follows a controlled prompt design.

Example prompt structure:

```
The doctor said that ___ would arrive soon.
```

Each occupation is prompted **multiple times** to observe consistency in pronoun assignment.

The model responses are then coded for:

* **he**
* **she**
* **they**
* pronoun avoidance (e.g. repetition of occupation titles)

This allows for quantitative comparison of gender representation across professions.

---

# Example Output

Example model completion:

```
The pilot said that he would land the plane shortly.
```

Extracted pronoun:

```
he
```

These outputs are aggregated to compute overall pronoun distributions.

---

# Key Findings

Preliminary results suggest that LLMs frequently associate:

* **technical or leadership roles** with male pronouns
* **caregiving professions** with female pronouns
* **neutral pronouns (they)** appear relatively rarely

These patterns suggest that LLM outputs may reflect **gender associations embedded in training data**.

---

# Skills Used

* Python
* OpenAI API
* Pandas
* Regex

---

# Research Context

This project was conducted as part of:

**HG2054: Pragmatics of AI Language**
Nanyang Technological University

The analysis applies concepts from:

* Gricean Pragmatics
* Conversational Implicature
* Normative Behaviour Theory
* Brown & Levinson’s Face Theory

to interpret gender assignment as a **pragmatic inference rather than a purely grammatical choice**.

---

# Disclaimer

This project is for academic research purposes.
The experiment analyzes model behavior and does not represent the author's views on gender or occupational roles.
