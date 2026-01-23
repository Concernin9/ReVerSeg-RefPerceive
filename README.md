# 🌟 ReVerSeg-RefPerceive  
**Training-Free Reason-and-Verify Framework for Language-Driven Traffic Video Segmentation**  

🚗 **Traffic Scene Understanding** &nbsp;|&nbsp; 🎯 **Language-Driven Segmentation** &nbsp;|&nbsp; 🧠 **Training-Free Inference**

---

<p align="center">
  <img src="assets/teaser.png" width="90%">
</p>

> **ReVerSeg** introduces a training-free *Reason-and-Verify* inference framework for robust language-driven traffic video segmentation.  
> We also present **Ref-Perceive**, a large-scale traffic-oriented benchmark with compositional referring instructions and frame-wise pixel annotations.

📄 Paper: *Under Review (IEEE T-ITS)*  
📦 Dataset & Code: **Will be released after paper acceptance**

---

## ✨ Highlights

- ✅ **Training-Free Inference Pipeline**  
  No fine-tuning. No additional data. Plug-and-play with foundation models.

- 🔍 **Semantic-Aware Keyframe Selection**  
  Automatically selects the most reliable frame for localization instead of using a fixed anchor.

- 🧪 **Two-Stage Verification Mechanism**  
  - Bounding-box level semantic verification  
  - Mask-level consistency verification  
  Effectively suppresses error propagation and identity drift.

- 🌍 **Traffic-Oriented Benchmark (Ref-Perceive)**  
  Covers multi-city, multi-weather, multi-illumination real-world traffic scenarios.

---

## 🧠 Method Overview: ReVerSeg

<p align="center">
  <img src="assets/pipeline.png" width="95%">
</p>

### 🔁 Training-Free Reason-and-Verify Pipeline

Compared with the traditional localization → propagation pipeline, ReVerSeg introduces structured inference-time control:

**Stage 1 — Semantic Keyframe Selection**  
Selects the most semantically reliable frame for target grounding.

**Stage 2-1 — Localization Verification**  
Checks whether predicted bounding boxes truly match the referring instruction.

**Stage 2-2 — Segmentation Verification**  
Validates mask-level semantic consistency to refine pixel predictions.

This design improves robustness **without modifying any foundation model parameters**.

---

## 📊 Ref-Perceive Dataset

<p align="center">
  <img src="assets/dataset_overview.png" width="90%">
</p>

### 📦 Dataset Summary

| Property | Value |
|---------|-------|
| Video Clips | **2,000** |
| Frames | **10,000** |
| Frames per Clip | **5** |
| Annotation Type | Pixel-level masks |
| Instruction Type | Compositional referring expressions |
| Domain | Real-world traffic scenes |

---

### 🌍 Geographic & Environmental Diversity

<p align="center">
  <img src="assets/world_map.png" width="85%">
</p>

Data collected across:

- 🇺🇸 New York, Chicago, Hollywood  
- 🇬🇧 London  
- 🇸🇬 Singapore  
- 🇨🇳 Harbin  

Conditions include:

- ☀️ Sunny  
- 🌧 Rainy  
- 🌙 Night  
- ❄️ Snow  

---

### 📝 Instruction Design

Ref-Perceive adopts **compositional referring expressions**, combining:

- Appearance  
- Spatial location  
- Object relations  
- Temporal consistency  
- Motion / state  

Example:

> *"Segment the white sedan driving in the center lane throughout all frames of the video."*

This design enforces **instance-level reasoning** and **cross-frame identity consistency**.

---

## 🧪 Experimental Results

<p align="center">
  <img src="assets/results.png" width="95%">
</p>

### 🚀 Performance Highlights

ReVerSeg consistently outperforms both:

- Image-based referring segmentation methods (GLAMM, LISA, UFO, PixelLM)
- Video-based baselines (VideoLISA, VISA, GLUS, VRS-HQ)

While preserving:

- Zero-shot generalization  
- Training-free deployment  
- Backbone-agnostic compatibility (Qwen2 / Qwen3 / InternVL)

---

## 📁 Code & Dataset Release Plan

⚠️ **Important Notice**

This repository currently serves as the **official project homepage for peer review**.

- 📦 Dataset: **Will be released after paper acceptance**
- 💻 Code: **Will be released after paper acceptance**
- 📑 Evaluation scripts and pretrained configurations will be provided together

We strictly follow journal data and code release policies.
