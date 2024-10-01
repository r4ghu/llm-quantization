# Optimizing LLMs through Quantization: A Hands-On Tutorial

This repository contains resources and code for **"Optimizing LLMs through Quantization: A Hands-On Tutorial"**, a session part of the Analytics Vidhya DataHour series. The focus of the tutorial is to explore the quantization of large language models (LLMs) to enhance deployment efficiency while maintaining model accuracy.

## Overview

Quantization is an essential technique in reducing the memory footprint and computational load of neural networks by converting the full-precision weights and activations to lower precision (e.g., 8-bit integers). This hands-on session will guide you through applying **Post-Training Quantization (PTQ)** and **Quantization-Aware Training (QAT)** on transformer models like BERT and GPT.

The repository includes code and Jupyter Notebooks for running experiments using quantization techniques on pre-trained LLMs, utilizing frameworks such as PyTorch and Hugging Face Transformers.

## Prerequisites

- **Machine Learning Knowledge**: Understanding of neural networks and model training.
- **Python Proficiency**: Ability to code in Python.
- **Familiarity with PyTorch and Hugging Face Transformers** (optional but recommended).
- Experience with **Jupyter Notebooks** for executing and visualizing experiments.

## Contents

- **Quantization Examples**: Notebooks demonstrating PTQ and QAT on 8-bit quantized LLMs.
- **Model Compression**: Techniques for compressing large models without compromising accuracy.
- **Performance Benchmarks**: Memory usage and inference speed comparisons between original and quantized models.

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/r4ghu/llm-quantization.git
   cd llm-quantization
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebooks to start the quantization experiments.

## Results

| **Model**              | **Accuracy (%)** | **Memory Footprint (MB)** |
|------------------------|------------------|---------------------------|
| 8-bit DistilBert        | 28.40            | 86.65                     |
| 8-bit DistilBert + LoRA | **92.35**            | **87.01**                     |
| Original DistilBert     | 92.70            | 255.43                    |

Quantization significantly reduces memory usage, and the use of LoRA helps in recovering most of the lost accuracy while keeping the model efficient.

## License

Licensed under the MIT License.