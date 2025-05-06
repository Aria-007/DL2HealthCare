# DL4HC_Project
# Reproducing Med-VQA: Visual Question Answering in Radiology

This repository contains the code, dataset references, and report for reproducing the Med-VQA task from the paper:

> Xu, Y., Liu, P., Zhang, H., et al. (2023). *Multi-modal Pre-training for Medical Vision-language Understanding and Generation*. Proceedings of CHIL 2023.

## 🔍 Project Overview

We evaluate the BLIP-2 model in a zero-shot setting on the VQA-RAD dataset and attempt lightweight fine-tuning. Our results highlight the difficulty of transferring general-purpose vision-language models to the medical domain.

## 📁 Folder Structure

- `BLIP2_VQA_RAD_Inference.ipynb` – Main Colab notebook for inference and fine-tuning attempts
- `VQA_RAD Dataset Public.json` – QA pairs used in inference
- `VQA_RAD Image Folder/` – Folder of de-identified radiology images
- `report/MedVQA_Report.pdf` – Final project report (single-column version)
- `report/MedVQA_Report_SingleColumn.tex` – Full LaTeX source

## 📊 Reproduced Results

- Subset: 50 samples from VQA-RAD
- **Exact Match Accuracy:** 0.00%
- Multiple failure types (wrong modality, organ confusion, hallucinations)

## 📦 Environment Setup

- Python 3.10
- Hugging Face Transformers
- PyTorch
- Colab T4 GPU

## 🚀 How to Run

1. Upload images and `.json` file to Colab
2. Run the `BLIP2_VQA_RAD_Inference.ipynb` notebook
3. Evaluate predictions via string match

## 📄 Final Report

[📄 Download the full report (PDF)](ADD_REPORT_LINK_HERE)

## 🙋 Author Contribution

This project was completed independently by **Aria Abrishamkar**.

---

## 📌 Notes

- This work was completed for the Deep Learning for Healthcare course (Spring 2025) at UIUC.
- Due to Colab limitations, only inference was performed; fine-tuning crashed due to GPU memory.

