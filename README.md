# 🌟 ReVerSeg-RefPerceive  
**Training-Free Reason-and-Verify Framework for Language-Driven Traffic Video Segmentation**

<p align="center">
  <img src="assets/teaser.png" width="850">
</p>

<p align="center">
  🚗 Traffic Scene Understanding &nbsp;|&nbsp; 🎯 Language-Driven Segmentation &nbsp;|&nbsp; 🧠 Training-Free Inference  
</p>

---

## 🏆 Highlights

- ⭐ **Training-Free Framework**: No additional training or fine-tuning is required  
- 🔍 **Reason-and-Verify Pipeline**: Explicit localization-level and mask-level verification  
- 🖼️ **Semantic-Aware Keyframe Selection**: Robust anchor frame discovery under complex traffic conditions  
- 📊 **Ref-Perceive Benchmark**: Multi-city, multi-condition traffic video dataset  

---

## 📌 Overview

**ReVerSeg** is a training-free inference framework designed for short-clip language-driven traffic video segmentation.
It improves robustness against semantic ambiguity and error propagation by introducing:

- Semantic-aware keyframe selection  
- Two-stage verification (bounding-box verification and mask verification)  
- Explicit reasoning and correction during inference  

This repository provides:

- ✅ Minimal runnable demo  
- ✅ Ref-Perceive-mini subset for reviewers  
- ⏳ Full dataset and full evaluation scripts will be released upon acceptance  


---

## 📂 Ref-Perceive-mini Dataset (Reviewer Release)

We release a lightweight subset for quick verification:

- 🎬 Short video clips (5 frames per clip)  
- 🏷️ Language referring instructions  
- 🖌️ Pixel-level segmentation masks  

📁 Location:
data/Ref-Perceive-mini/
