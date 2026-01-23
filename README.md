# 🌟 ReVerSeg-RefPerceive  
**Training-Free Reason-and-Verify Framework for Language-Driven Traffic Video Segmentation**

<p align="center">
  <img src="fig/title(1)_01.jpg" width="850">
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

  
<p align="center">
  <img src="fig/comp-video-1_01.jpg" width="80%">
</p>

> **ReVerSeg** introduces a training-free *Reason-and-Verify* inference framework for robust language-driven traffic video segmentation.  
> We also present **Ref-Perceive**, a large-scale traffic-oriented benchmark with compositional referring instructions and frame-wise pixel annotations.

📄 Paper: *Under Review*  
📦 Dataset & Code: **Will be released after paper acceptance**


---

## 📊 Ref-Perceive Dataset

<p align="center">
  <img src="fig/zipdataset-0118-2_01(1).jpg" width="80%">
</p>


---

### 🌍 Geographic & Environmental Diversity

<p align="center">
  <img src="fig/world-1_01.jpg" width="65%">
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


## 🚀 Performance Highlights

ReVerSeg consistently outperforms both:

- Image-based referring segmentation methods 
- Video-based baselines

While preserving:

- Zero-shot generalization  
- Training-free deployment  
- Backbone-agnostic compatibility

---

## 📁 Code & Dataset Release Plan

⚠️ **Important Notice**

This repository currently serves as the **official project homepage for peer review**.

- 📦 Dataset: **Will be released after paper acceptance**
- 💻 Code: **Will be released after paper acceptance**
- 📑 Evaluation scripts and pretrained configurations will be provided together

We strictly follow journal data and code release policies.
