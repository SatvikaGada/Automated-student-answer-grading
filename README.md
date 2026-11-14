# Automated Student Answer Grading (ASAG) Pipeline

An end-to-end Natural Language Processing (NLP) pipeline designed to evaluate, score, and analyze student short-answers against reference answers using semantic similarity, lexical overlap, and readability metrics.

---

## Overview

Automated Student Answer Grading (ASAG) systems assist educators by automatically evaluating student free-text responses against human-graded reference benchmarks. This project utilizes a combination of vector embeddings, cosine similarity, relative length metrics, and lexical matching to predict and evaluate student scores.

---

## Features

- **Semantic Similarity:** Computes vector embedding and TF-IDF cosine similarity between student submissions and reference answers.
- **Text Preprocessing & Lemmatization:** Utilizes spaCy for tokenization, stop-word removal, and lemmatization.
- **Lexical & Structural Analysis:** Evaluates N-gram overlap ratios and length ratios to capture syntactic alignment.
- **Exploratory Data Analysis:** Generates statistical comparisons and visualizations across human-assigned grade tiers.

---

## Dataset Description

The datasets contain student responses paired with reference answers and human evaluation scores. Key columns include:

- `question`: The prompt text presented to the student.
- `student_answer`: The raw response submitted by the student.
- `ref_answer`: The ground-truth reference answer.
- `grades_round`: Human-assigned evaluation grade.
- `cos_similarity`: Computed cosine similarity score between answer embeddings.
- `length_ratio`: Ratio of student answer length relative to the reference answer.

---

## Installation and Prerequisites

Ensure you have Python installed, then install the required dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn spacy textstat
python -m spacy download en_core_web_sm
```
