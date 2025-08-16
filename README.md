# Building GPT-2 From Scratch (PyTorch)

This repository is my personal journey of building GPT-2 completely from scratch, no shortcuts, just pure Python + PyTorch.  

I wanted to truly understand how LLMs actually work under the hood, and not just treat them as "black boxes." Inspired by Dr. Raj Abhijit Dandekar’s incredible tutorial series and the book *Build a Large Language Model* by Sebastian Raschka, I decided to code everything line by line.

---

## 📂 What’s Inside

### 1. `pretraining/`
This folder contains the **full GPT-2 architecture and pretraining code**, built completely from scratch.  
- Dataset: [TinyStories](https://huggingface.co/datasets/roneneldan/TinyStories) (~460M tokens)  
- Config: Modified GPT-2 (fewer heads, reduced embedding dimension, shorter context length) to fit GPU constraints  
- GPU Used: RTX 4090  
- Training: ~2 hours, ~4 epochs  
- Output: Surprisingly coherent and grammatically sound short stories

### 2. `tutorial_walkthrough/`
This folder is more of a **learning resource** than a training script.  
It contains the **step-by-step implementation of GPT-2 coded alongside the tutorial**, with incremental explanations at every stage:  
- Embeddings  
- Attention mechanism  
- Why we divide attention scores by `sqrt(head_dim)`  
- Transformer blocks  
- Final model assembly  

Think of it as “learning with me” code, if you’re new to LLM internals, this will help you see the architecture evolve piece by piece.

---

## Acknowledgements
- [Dr. Raj Abhijit Dandekar](https://www.youtube.com/watch?v=Xpr8D6LeAtw&list=PLPTV0NXA_ZSgsLAr8YCgCwhPIJNNtexWu) for the amazing playlist that sparked this journey  
- [Sebastian Raschka](https://sebastianraschka.com/) for *Build a Large Language Model from Scratch*  

---

