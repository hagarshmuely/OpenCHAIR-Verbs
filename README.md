# OpenCHAIR-Verbs

**An extension of [OpenCHAIR](https://huggingface.co/papers/2312.03631) focused on verb-centric action understanding in image captioning**

---

## Overview

**OpenCHAIR-Verbs** builds on the [OpenCHAIR benchmark](https://huggingface.co/papers/2312.03631) introduced by Ben-Kish et al. (EMNLP 2024), which evaluates hallucinations in open-vocabulary image captioning. While OpenCHAIR focuses on **object hallucination**, OpenCHAIR-Verbs shifts the focus to **verbs and actions**—critical for evaluating how well captioning models describe **what is happening** in an image.

---

## 🎯 Motivation

- Extend the OpenCHAIR benchmark to **action understanding**, not just object recognition
- Evaluate models’ ability to **correctly ground verbs** in generated captions
- Provide a **verb-centric synthetic benchmark** for analyzing hallucinations and misinterpretations in dynamic scenes


---
## 🌐 Public Dataset on Hugging Face

We also publish a cleaned and validated verb-centric subset under the name:

**`Hagarsh/OpenCHAIR_verb`** — a curated image‑caption dataset focused on high-quality verb grounding and action semantics.

## 📦 Repository Structure

- `verb_captions/` — Captions designed around diverse action verbs
- `generate_images.py` — Generate images from verb-centric captions using image generation models (e.g., SDXL)
- `save_dataset_hf.py` — Save image-caption dataset in Hugging Face format
- `human_validation.py` — Script for collecting and processing human validation of generated actions
- `caption_images_with_different_models.ipynb` — Caption generated images using different models for evaluation
- `llm_compare_captions.py` — LLM-based comparison of model captions to reference descriptions

---

## 🚀 Environment Setup

### 1. Clone the repository

```bash
conda env create -f environment.yml
conda activate mocha
```
