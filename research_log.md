# Research Log

## 2026-10-01 — Dataset Design

### Objective
Create a small Urdu dataset to investigate whether Qwen can understand
sarcasm, culturally implicit responses, and indirect meanings in Urdu.

### Dataset Categories
- Sarcasm
- Culturally Implicit Meaning
- Indirect Meaning

### Dataset Structure
Each example contains:
- ID
- Category
- Urdu text
- English translation
- Urdu context
- English context
- Urdu question
- English question
- Expected interpretation in Urdu
- Expected interpretation in English

### Experimental Decision
The model-facing input will contain only the Urdu text, Urdu context,
and Urdu question. English translations will be kept for documentation
and human evaluation.

### Reason
Using Urdu for the model-facing input allows the experiment to focus
on Urdu language and implicit-meaning understanding rather than mixing
Urdu input with English instructions.