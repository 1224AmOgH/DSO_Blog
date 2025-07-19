---
title: "Deep Sky Object Detection with Deep Learning"
author: "Seminar Blog"
date: 2025-07-19
layout: post
---

# Introduction

With the growth of smart telescopes capable of Electronically Assisted Astronomy (EAA), astronomy is becoming more accessible to hobbyists and the public. Yet, detecting faint galaxies, nebulae and clusters in light-polluted skies remains a persistent challenge. The paper _"Deep Sky Objects Detection with Deep Learning for Electronically Assisted Astronomy"_ by Parisot & Jaziri tackles this head-on—crafting deep learning (DL) solutions that help in real-time detection of celestial wonders.

In this blog, we explore a range of deep learning techniques developed for detecting Deep Sky Objects (DSOs) in images captured by smart telescopes, comparing their strengths and weaknesses and reflecting on real-world applications.

# Background: From Eyepieces to Algorithms

Stargazing historically required remote locations, patience, and complex equipment. EAA has changed that — replacing eyepieces with digital sensors like those in Stellina and Vespera smart telescopes, enabling real-time image stacking even from urban environments. But these do not identify what’s in the image — users must still know astronomy or consult charts.

# Current Limitations in EAA

1. **Image Ambiguity** – DSOs often blend into stars/noise.
2. **No Real-Time Feedback** – No confirmation if objects are captured.
3. **Environmental Sensitivity** – Image quality varies with conditions.
4. **Lack of Annotation** – No automatic labeling of celestial targets.

# High-Level Deep Learning Pipeline

1. **Raw Image** – Captured by telescope; typically RGB or FITS.
2. **DL Model** – Detects DSOs using YOLO/ResNet/GAN.
3. **Annotations** – Bounding boxes, heatmaps, catalog labels.
4. **Understanding** – Visual cues for non-experts (possibly with XRAI).

# Data Collection

Captured with Stellina and Vespera telescopes (2022–2023) across Luxembourg, France, and Belgium — ~50,000 raw FITS and 5,000 JPEGs representing over 250 targets.

# Detection Techniques

## Technique 1: StarNet + Computer Vision

Removes stars → applies grayscale + Canny edge → finds DSOs.  
**Pros:** Fast, simple  
**Cons:** Noise-sensitive, low accuracy

## Technique 2: YOLOv7 Object Detection

Custom-trained on ~4,700 annotated images.  
**F1 Score:** 0.62 (Best)  
**Pros:** Real-time, accurate, scalable  
**Cons:** Misses small/faint DSOs, requires labeled data

## Technique 3: ResNet50 + XRAI

Binary classifier + explainable heatmaps via Integrated Gradients.  
**F1 Score:** 0.51  
**Pros:** Highly interpretable  
**Cons:** Slower, lacks real-time bounding boxes

## Technique 4: Pix2Pix GAN

Trained to imitate XRAI heatmaps from telescope images.  
**Pros:** Fast feedback, low compute  
**Cons:** Approximate, no object classification

# Summary Table

| Aspect     | YOLOv7                | ResNet + XRAI            | Pix2Pix GAN              |
|------------|------------------------|---------------------------|---------------------------|
| Goal       | Detect + Localize DSO  | Classify + Explain (XAI)  | Generate highlight maps   |
| Output     | Bounding boxes         | Binary + Heatmap          | XRAI-style heatmaps       |
| Speed      | Real-time              | Slow                      | Fast                      |
| Explainable| ❌                    | ✅                        | ✅ (approximate)         |
| F1 Score   | **0.62**               | 0.51                      | PSNR > 38                |

# Applications of DL in EAA

- Smart real-time detection (YOLO, ResNet)
- Post-capture filtering and annotation
- Explainability for user trust (XRAI)

# Limitations

- Domain-specific datasets reduce generalizability
- High compute cost (XRAI especially)
- Detection ambiguity for faint or noisy DSOs
- No common benchmark for fair model comparison

# Future Work

### Improve ResNet50 + XRAI
- Tune hyperparameters, improve architecture (EfficientNet)
- Better labeling, Grad-CAM++ explainability

### Improve YOLOv7
- Train for multiple DSO classes
- Use augmentation for robustness

# Conclusion

Deep learning turns smart telescopes into intelligent, interactive observatories. YOLOv7 delivers the best detection, ResNet + XRAI explains decisions, and Pix2Pix offers speed. Future improvements will bring more accuracy, explainability, and accessibility — bringing astronomy closer to everyone.

> Deep learning isn’t just showing us the stars — it’s helping us understand them.
