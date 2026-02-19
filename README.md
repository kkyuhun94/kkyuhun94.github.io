# Jung Kyu Heon

Data-Centric AI Researcher  
Leveraging Foundation Models to Address Data Scarcity

---

## 👋 About Me

I am a PhD candidate in Industrial & Data Engineering at Pukyong National University (TEAMLAB).

My research focuses on **Data-Centric AI**, particularly how Foundation Models (LLMs and Diffusion Models) can be used as controllable synthetic data generators to address qualitative data deficiencies in low-shot learning scenarios.

Rather than scaling model size indefinitely, I focus on:

- Improving data quality
- Designing controllable synthetic data pipelines
- Aligning augmentation strategies with downstream objectives
- Ensuring reproducibility and modularity

I view data scarcity not merely as a quantitative limitation, but as a qualitative gap in representation.

---

## 🎯 Research Interests

- Synthetic Data
- Data Augmentation
- Few-shot Image Classification
- Diffusion Models
- Large Language Models
- Data Distribution Control
- Multilingual & Cultural AI
- AI Safety & Dataset Construction

---

# 🔬 Research

---

## 1️⃣ DALDA  
**Data Augmentation Leveraging Diffusion Model and LLM with Adaptive Guidance**  
(ECCVW 2024 – Oral)

### Problem

- Few-shot learning suffers from limited diversity.
- Text-only Diffusion prompting risks class inconsistency.
- Fine-tuning Diffusion Models is computationally expensive.

### Approach

- LLM generates context-rich prompts.
- IP-Adapter enables reference-guided generation.
- CLIP-based Adaptive Guidance Scaling:

  - Low CLIPScore → Increase guidance → Reduce diversity  
  - High CLIPScore → Decrease guidance → Increase diversity  

This dynamically balances diversity and fidelity.

### Results

- +9.07%p average improvement in 1-shot classification
- Evaluated on multiple benchmarks
- Presented at ECCVW 2024 (Oral)

**Keywords:** Synthetic Data, Diffusion Model, LLM, CLIP, Few-shot Learning

---

## 2️⃣ CABIN  
**Controlling Augmentations for Balancing Invariance and Diversification in One-Shot Image Classification**  
(Under Review)

### Core Insight

Diversity and Fidelity should not be optimized simultaneously.  
They should be separated and aligned with training stages.

### Two-Type Augmentation

**1. Diversity-focused synthesis**
- Rich contextual prompts
- Low image guidance
- Broad distribution coverage

**2. Key feature-focused synthesis**
- Class-defining attributes
- Higher guidance
- Strong class consistency

### Two-Stage Training

- Stage 1: Broad representation learning  
- Stage 2: Class fidelity refinement  

### Contribution

- Stable across different LLMs and Diffusion backbones
- Modular synthetic data framework
- Reduced sensitivity to model choice

**Keywords:** Synthetic Data, Data Distribution, Invariance, Diversity, Multi-stage Learning

---

## 3️⃣ KoDi  
**A Korean Diffusion Model for Bilingual Text-to-Image Generation and Cultural Fidelity**  
(IEEE Access)

### Problem

- Most Diffusion Models are trained on English/Chinese data.
- Korean cultural concepts are underrepresented.
- Cultural evaluation metrics are insufficient.

### Contributions

1. Korean Cultural Dataset (KCD) construction  
2. Multilingual prompting:
   - Korean
   - Phonetic English (Romanization)
   - Semantic English translation  
3. Cultural evaluation pipeline:
   - KC-CLIP similarity
   - LVLM-based country identification  

### Results

- Improved cultural fidelity over multilingual baselines
- Human + automatic evaluation improvements

**Keywords:** Multilingual Diffusion Model, Cultural Adaptation, Dataset Curation

---

## 4️⃣ Pseudo Outlier Exposure  
**Out-of-Distribution Detection without External Data**  
(ACL 2023 Findings)

### Problem

OOD detection typically requires external OOD data.

### Solution

- Mask high-attention tokens
- Generate surrogate OOD samples
- Train rejection network

### Result

- Competitive AUROC & F1
- No external OOD data required

**Keywords:** NLP, OOD Detection, Transformer, Surrogate Data Generation

---

## 5️⃣ Ko-ToxicWebQ  
**A Korean Toxic Web Query Dataset**  
(Under Review)

### Motivation

- Toxic query detection benchmarks are English-centric.
- Korean obfuscation detection remains underexplored.

### Contributions

- 47.7K real Korean search queries
- 7 toxicity categories
- 3 obfuscation categories
- Korean-specific benchmark

**Keywords:** AI Safety, Dataset Construction, Toxic Query Detection

---

# 🧪 Applied & Industrial Projects

---

## 🔥 FireFusion (Patent)

Diffusion-based synthetic fire image generation system.

- LoRA fine-tuning
- ControlNet masking
- BLIP captioning + GPT recaptioning
- Improved detection training performance over traditional augmentation

---

## 🌍 Patent Domain NMT

mBART fine-tuned for patent translation.

- Domain adaptation
- Back translation
- Improved BLEU & TER scores

---

## 🏭 SYnet

4D CNN-based demand prediction model for shipyard maintenance vehicles.

- Spatial + temporal modeling
- Industrial deployment context
- Published in Industrial Engineering & Manufacturing Systems

---

# 📚 Publications

## Journal
- KoDi – IEEE Access
- SYnet – Industrial Engineering & Manufacturing Systems

## Conference
- Pseudo Outlier Exposure – ACL 2023
- DALDA – ECCVW 2024

## Under Review
- CABIN
- Ko-ToxicWebQ

---

# 🛠 Technical Stack

## Foundation Models
- GPT-4o
- GPT-4.1
- GPT-5
- Stable Diffusion 1.5
- SDXL

## Vision Models
- ResNet50
- ViT-B/16
- ViT-L/16
- CLIP

## Training Strategy
- Multi-stage learning
- Few-shot fine-tuning
- Descriptor-based prompt construction
- Synthetic data integration

## Infrastructure
- NVIDIA H100 GPUs
- PyTorch
- Hugging Face ecosystem

---

# 📈 Research Trajectory

My research evolves around a central question:

**How can Foundation Models be used as controllable data generators to bridge qualitative gaps in low-resource learning?**

- DALDA addressed diversity control.
- CABIN structured augmentation control.
- KoDi extended the framework to cultural fidelity.
- Ko-ToxicWebQ expands into AI safety and data governance.

---

# 📎 Links

Google Scholar: https://scholar.google.com/citations?user=gJSM26UAAAAJ&hl=en  
GitHub: https://github.com/kkyuhun94  
Email: kkyuhun94@gmail.com

---

Thank you for visiting.
