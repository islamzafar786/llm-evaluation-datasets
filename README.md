# LLM Evaluation Datasets  
This repository is part of the research project *“Can LLMs Generate Bachelor’s or Master’s Thesis Ideas?”*..
This repository contains the complete resulted datasets created by Large Language Models (LLMs) based on given valid and bad thesis-ideas dataset during an evaluation.  
It includesthe **LLM-generated evaluation results** for four metrics:

- **Clarity**
- **Novelty**
- **Feasibility**
- **Validness**

---

## Repository Structure

### 1. **Valid examples tested results/**
Contains all *LLM-generated scoring results* for **42 valid thesis ideas**, across all four metrics and models.  
Each file is in JSON format.

Example models:
- Mistral-7B  
- Mistral-24B  
- Llama-3-8B  
- Gemma-3-4B  
- QWQ-32B  

Each JSON contains:
- model-generated score (1–5)
- rationale text
- metric-specific sub-scores  
- pass/fail mapping  
- normalized JSON structure

---
### 2. **Bad examples tested results/**
Contains all *evaluation results* for the **9 bad thesis ideas**, where each idea is labeled with the metric(s) it should fail.  

These files were used for:
- overall accuracy  
- true-fail detection (recall on failing metrics)  
- non-target correctness (specificity)

---

### 3. **Evaluation related Insights/**
Contains high-level PDF summaries generated from the model results:
- per-model insights  
- metric-wise distribution  
- cross-metric observations  
- strengths/weaknesses of each LLM  

These PDFs are used to support the evaluation chapter in the research paper.

### 4. **Valid and Bad thesis ideas with sources.pdf**
This document contains:
- all **original 42 valid ideas**  
- all **9 bad ideas**  
- their textual descriptions  
- source links  
- topic categorization  

This is the *ground-truth dataset* used to perform all evaluations.

## Evaluation Summary
The datasets in this repository were used to evaluate whether LLMs can accurately assess thesis-idea quality under four academic metrics.  

Each LLM returned:
- a 1–5 score  
- rationale text  
- optional sub-metric scores (for clarity testing)  

Accuracy was calculated separately for:
- **Valid ideas (42)**  
- **Bad ideas (9)** including true-fail detection and non-target metric handling  

---

## Usage
You can use these JSON datasets to:
- reproduce the evaluation process  
- test new LLM models  
- train custom scoring models  
- analyze model-specific judgment patterns  
- benchmark your own evaluation pipeline  

---

## License
This dataset is released for academic and research use.  
If used, please cite the associated project/research work.

---

## Contributors
- Anastasia
- Islam Zafar  
- Abishek  
- Supervisors (Marburg University)


