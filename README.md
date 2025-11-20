# 🌈 Gray to RGB — Deep Image Colorization Suite  
### *ECCV16 + SIGGRAPH17 Models · PyTorch · Streamlit App (Offline)*  

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red.svg)]()
[![Streamlit](https://img.shields.io/badge/Streamlit-App-green.svg)]()
![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)

A complete offline tool for colorizing grayscale images using the **official ECCV16** and **SIGGRAPH17** models by **Richard Zhang et al.**  
Run both models side-by-side, compare outputs visually, download the results, and explore dominant color palettes — all inside an interactive Streamlit UI.

---

# 📌 Table of Contents

- [✨ Overview](#-overview)  
- [🎯 Goal & Problem Definition](#-goal--problem-definition)  
- [📂 Repository Structure](#-repository-structure)  
- [⭐ Features](#-features)  
- [🧰 Tech Stack](#-tech-stack)  
- [📦 Requirements](#-requirements)  
- [⚙️ Installation](#️-installation)  
- [▶️ Running the App](#️-running-the-app)  
- [🖼️ Screenshots](#️-screenshots)  
- [📥 Optional: Download Kaggle Dataset](#-optional-download-kaggle-dataset)  
- [🔄 Workflow Pipeline](#-workflow-pipeline)  
- [🛠️ Customization Ideas](#️-customization-ideas)  
- [🐞 Troubleshooting](#-troubleshooting)  
- [📜 License](#-license)  
- [🙏 Credits](#-credits)

---

# ✨ Overview

This project provides a **local playground** for exploring two classic deep-learning colorization models:

- **ECCV16** (Classification-based 313-color bins)  
- **SIGGRAPH17** (Colorization with local + global hints)

Both models are provided as **pretrained PyTorch checkpoints**, and the Streamlit UI makes the process easy:

✔ Upload grayscale or RGB image  
✔ Auto-convert to LAB  
✔ Run both models  
✔ View side-by-side results  
✔ Download colorized outputs  
✔ Inspect dominant colors  

---

# 🎯 Goal & Problem Definition

### **🎯 Goal**
To offer an *offline*, easy-to-use UI for experimenting with deep image colorization models.

### **🧠 Problem Definition**
Given an image in grayscale (or RGB → Luminance), infer plausible **chrominance channels (`a/b`)** using CNNs trained on millions of natural images.  
This repo focuses specifically on **inference**, not training.

---

# 📂 Repository Structure

