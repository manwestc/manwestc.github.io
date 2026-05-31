---
layout: single
published: true
title: "Introduction to TINTOlib: Unlocking the Power of Vision Architectures for Tabular Data"
date: 2026-05-27
last_modified_at: 2026-05-27
permalink: /blog/2026/05/01-introduction-to-tintolib-tabular-to-image/
author_profile: true
read_time: true
share: true
related: true
classes: wide-blog-post
category: "TINTOlib"
categories:
  - TINTOlib
tags:
  - TINTOlib
  - Tabular-to-Image
  - Synthetic Images
  - Deep Learning
  - CNN
  - PyTorch
  - Machine Learning
description: "Technical introduction to TINTOlib, a Python framework for transforming tabular data into synthetic images and applying CNN-based deep learning architectures."
excerpt: "Technical introduction to TINTOlib, a Python framework for transforming tabular data into synthetic images and applying CNN-based deep learning architectures."
image: "/images/Blog/2026-05-27-01-introduction-to-tintolib-tabular-to-image.png"
header:
  teaser: "/images/Blog/2026-05-27-01-introduction-to-tintolib-tabular-to-image.png"
---

<link rel="canonical" href="{{ site.url }}{{ page.url }}">
<meta name="robots" content="index,follow,max-image-preview:large">
<meta name="description" content="{{ page.description }}">

<meta property="og:type" content="article">
<meta property="og:title" content="{{ page.title }}">
<meta property="og:description" content="{{ page.description }}">
<meta property="og:url" content="{{ site.url }}{{ page.url }}">
<meta property="og:image" content="{{ site.url }}{{ page.image }}">
<meta property="article:published_time" content="{{ page.date | date_to_xmlschema }}">
<meta property="article:modified_time" content="{{ page.last_modified_at | default: page.date | date_to_xmlschema }}">
<meta property="article:author" content="Manuel Castillo-Cara">
<meta property="article:section" content="{{ page.category }}">
{% for tag in page.tags %}
<meta property="article:tag" content="{{ tag }}">
{% endfor %}

<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="{{ page.title }}">
<meta name="twitter:description" content="{{ page.description }}">
<meta name="twitter:image" content="{{ site.url }}{{ page.image }}">

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BlogPosting",
  "headline": {{ page.title | jsonify }},
  "description": {{ page.description | jsonify }},
  "image": "{{ site.url }}{{ page.image }}",
  "author": {
    "@type": "Person",
    "name": "Manuel Castillo-Cara",
    "url": "{{ site.url }}/"
  },
  "publisher": {
    "@type": "Person",
    "name": "Manuel Castillo-Cara",
    "url": "{{ site.url }}/"
  },
  "datePublished": "{{ page.date | date_to_xmlschema }}",
  "dateModified": "{{ page.last_modified_at | default: page.date | date_to_xmlschema }}",
  "mainEntityOfPage": {
    "@type": "WebPage",
    "@id": "{{ site.url }}{{ page.url }}"
  },
  "articleSection": {{ page.category | jsonify }},
  "keywords": {{ page.tags | join: ", " | jsonify }}
}
</script>

<div style="background: linear-gradient(135deg, #1a237e 0%, #4a148c 50%, #311b92 100%); border-radius: 12px; padding: 2.5rem 2rem; margin: 1.5rem 0 2.5rem; display: flex; flex-wrap: wrap; align-items: center; gap: 2rem; color: #fff;">
  <div style="flex: 1 1 280px; min-width: 0;">
    <p style="margin: 0 0 0.4rem; font-size: 0.78rem; letter-spacing: 0.12em; text-transform: uppercase; color: #b39ddb; font-weight: 600;">TINTOlib · Deep Learning · Tabular-to-Image</p>
    <h1 style="margin: 0 0 0.75rem; font-size: clamp(1.5rem, 4vw, 2.1rem); font-weight: 800; line-height: 1.2; color: #fff;">Introduction to TINTOlib</h1>
    <p style="margin: 0 0 1rem; font-size: 0.97rem; color: #e1d5f5; line-height: 1.55;">A Python framework for transforming tabular data into synthetic images and applying CNN-based vision architectures — bridging the gap between structured data and deep learning.</p>
    <div style="display: flex; flex-wrap: wrap; gap: 0.5rem;">
      <span style="background: rgba(255,255,255,0.15); border-radius: 20px; padding: 0.25rem 0.75rem; font-size: 0.78rem; color: #e8d5ff;">PyTorch</span>
      <span style="background: rgba(255,255,255,0.15); border-radius: 20px; padding: 0.25rem 0.75rem; font-size: 0.78rem; color: #e8d5ff;">CNN</span>
      <span style="background: rgba(255,255,255,0.15); border-radius: 20px; padding: 0.25rem 0.75rem; font-size: 0.78rem; color: #e8d5ff;">Tabular Data</span>
      <span style="background: rgba(255,255,255,0.15); border-radius: 20px; padding: 0.25rem 0.75rem; font-size: 0.78rem; color: #e8d5ff;">Synthetic Images</span>
    </div>
  </div>
  <div style="flex: 0 0 auto; max-width: 260px; width: 100%;">
    <img src="/images/Blog/2026-05-27-01-introduction-to-tintolib-tabular-to-image.png" alt="TINTOlib tabular-to-image transformation" style="width: 100%; border-radius: 10px; box-shadow: 0 8px 32px rgba(0,0,0,0.45); display: block;">
  </div>
</div>

---

>> - **Author:** Manuel Castillo-Cara, PhD
>> - **Affiliation:** Dpt. of Artificial Intelligence, Universidad Nacional de Educación a Distancia (UNED), Spain
>> - **Role:** Researcher, Professor, and TINTOlib Python Library Developer
>> - **License:** [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) unless otherwise stated.

---

In contemporary Data Science, an established paradigm governs model selection: Deep Learning architectures dominate unstructured modalities such as computer vision and natural language processing, whereas gradient-boosted decision trees (GBDTs)—including **XGBoost**, **LightGBM**, and **CatBoost**—remain the gold standard for structured tabular datasets. 

However, recent advancements in deep learning have challenged this dichotomy through the introduction of **spatial encoding techniques**. By transforming tabular features into synthetic multi-dimensional images, researchers can leverage the structural inductive biases of advanced computer vision networks, such as Convolutional Neural Networks (CNNs) and Vision Transformers (ViTs). This article provides a comprehensive theoretical and practical introduction to **TINTOlib**, the state-of-the-art Python library designed to streamline this transformation pipeline.

## The Theoretical Framework: Why Map Tables to Images?

The primary impediment to directly applying CNNs to tabular datasets is the **absence of spatial locality**. In natural images, adjacent pixels exhibit strong semantic and structural correlations (e.g., forming edges, textures, and continuous geometric shapes). Conversely, rows and columns in a standard tabular matrix possess an arbitrary ordering; swapping column 2 and column $d$ changes the array indices but preserves the underlying data semantics. This structural format violates the **spatial inductive bias**—specifically, translation invariance and locality—upon which convolutional filters rely.

To overcome this limitation, spatial encoding methodologies project the feature space onto a discrete 2D coordinate system. Features that exhibit strong statistical correlations or mutual dependencies are mapped to proximal spatial coordinates within a synthetic "canvas," generating a **synthetic pseudo-image**.

![Tabular Data into Synthetic Images Methodology](/images/Blog/2026-05-27-01-introduction-to-tintolib-tabular-to-image.png)
*(Figure 1: Conceptual diagram illustrating the topological mapping of tabular feature vectors into a structured 2D pixel grid via TINTOlib spatial encoding).*

Through this transformation, the vision model's convolutional kernels can extract higher-order hierarchical feature interactions. Furthermore, this paradigm shifts tabular analysis from black-box numeric mapping to a visual space, enabling the direct integration of post-hoc Explainable AI (XAI) frameworks—such as **Grad-CAM**, **SHAP**, or **PermGrad**—to visually interpret feature attributions via saliency maps.

## What is TINTOlib?

**[TINTOlib](https://github.com/oeg-upm/TINTOlib)** is an open-source Python framework that unifies a comprehensive suite of state-of-the-art tabular-to-image transformation algorithms under a single, cohesive, Scikit-Learn-compliant interface. For a comprehensive overview of the framework's capabilities, consult the official **[TINTOlib Documentation](https://tintolib.readthedocs.io/en/latest/)**.

Historically, evaluating different spatial encoding strategies required integrating disjointed, unstandardized repositories written across varying programming languages. TINTOlib resolves this fragmentation by categorizing and implementing both parametric and non-parametric approaches. While this tutorial focuses on the **TINTO** method (which utilizes manifold learning techniques like t-SNE or Principal Component Analysis to determine spatial feature positions), the library allows researchers to pivot to **any other methodology**—such as **IGTD**, **REFINED**, **SuperTML**, **BarGraph**, or **Binary Image Encoding (BIE)**—by modifying a single line of code, ensuring a seamless benchmarking experience.

## Practical Implementation: Building Your First PyTorch CNN Pipeline

To demonstrate the efficacy of this paradigm, we will construct an end-to-end classification pipeline. To ensure strict reproducibility, we will utilize the standard *Breast Cancer Wisconsin* dataset from Scikit-Learn.

### 1. Spatial Encoding and Data Leakage Mitigation

A critical methodological vulnerability in spatial encoding is **Data Leakage**. Algorithms that learn the optimal spatial arrangement of pixels based on feature similarities (such as t-SNE, PCA, or distance-matrix optimizations) must **never** be exposed to the validation or testing partitions during the fitting phase. Doing so allows the topological properties of the unseen test data to influence the coordinate mapping, invalidating subsequent generalization metrics.

To ensure rigorous validation, the pipeline must strictly segregate data prior to mapping: call `.fit()` exclusively on the training partition to define the spatial configuration, and subsequently apply `.transform()` to generate the synthetic images for both sets independently.

```python
import pandas as pd
from sklearn.datasets import load_breast_cancer
from sklearn.model_selection import train_test_split
from TINTOlib.tinto import TINTO

# 1. Load the structured tabular dataset (Breast Cancer - 30 numeric features)
raw_data = load_breast_cancer()
df = pd.DataFrame(raw_data.data, columns=raw_data.feature_names)
# Append the target variable as the final column, conforming to tidy data standards
df['target'] = raw_data.target 

# 2. Partition the dataset to guarantee strict validation boundaries
X_train, X_test = train_test_split(df, test_size=0.2, random_state=42)

# 3. Instantiate the spatial encoder (TINTO via t-SNE optimization, outputting a 20x20 canvas)
# Note: To alternate methods, simply import and instantiate IGTD or REFINED here.
encoder = TINTO(problem="supervised", algorithm="t-SNE", pixels=20, blur=True)

# 4. Fit the spatial coordinate mapping matrix ONLY using the training split
encoder.fit(X_train)

# 5. Transform the tabular matrices into synthetic image repositories
encoder.transform(X_train, "synthetic_dataset/train/")
encoder.transform(X_test, "synthetic_dataset/test/")
print("Transformation completed successfully. Spatial representations isolated.")
```

<div style="display: flex; gap: 0.75rem; justify-content: center; flex-wrap: wrap; margin: 1.5rem 0 0.5rem;">
  <img src="/images/Blog/synthetic_images/2026-05-27-01_TINTO1.png" alt="Synthetic image 1 generated by TINTOlib TINTO with blurring" style="width: 120px; height: 120px; object-fit: contain; border: 1px solid #e2e8f0; border-radius: 4px; background: #f8fafc;">
  <img src="/images/Blog/synthetic_images/2026-05-27-01_TINTO2.png" alt="Synthetic image 2 generated by TINTOlib TINTO with blurring" style="width: 120px; height: 120px; object-fit: contain; border: 1px solid #e2e8f0; border-radius: 4px; background: #f8fafc;">
  <img src="/images/Blog/synthetic_images/2026-05-27-01_TINTO3.png" alt="Synthetic image 3 generated by TINTOlib TINTO with blurring" style="width: 120px; height: 120px; object-fit: contain; border: 1px solid #e2e8f0; border-radius: 4px; background: #f8fafc;">
</div>
*(Figure 2. Synthetic image samples generated with TINTOlib using the TINTO method with blurring. Each image corresponds to an individual tabular instance from the Breast Cancer Wisconsin dataset and encodes its feature values into a two-dimensional spatial representation. The resulting intensity patterns can be processed by CNN-based and hybrid neural architectures.)*

### 2. Architectural Specification in PyTorch

Following image generation, we construct a standard Convolutional Neural Network tailored to ingest the single-channel (grayscale) $20 \times 20$ pixel representations yielded by TINTOlib.

```python
import torch
import torch.nn as nn
import torch.nn.functional as F

class TabularCNN(nn.Module):
    def __init__(self, num_classes=2):
        super(TabularCNN, self).__init__()
        
        # Convolutional Block 1: Input channels = 1, Output feature maps = 32
        self.conv1 = nn.Conv2d(in_channels=1, out_channels=32, kernel_size=3, padding=1)
        self.pool1 = nn.MaxPool2d(kernel_size=2, stride=2)
        
        # Convolutional Block 2: Input channels = 32, Output feature maps = 64
        self.conv2 = nn.Conv2d(in_channels=32, out_channels=64, kernel_size=3, padding=1)
        self.pool2 = nn.MaxPool2d(kernel_size=2, stride=2)
        
        # Given a 20x20 input, two successive MaxPool reductions yield a 5x5 spatial size
        self.flatten = nn.Flatten()
        self.fc1 = nn.Linear(64 * 5 * 5, 128)
        self.fc2 = nn.Linear(128, num_classes)

    def forward(self, x):
        # Block 1 forward pass
        x = self.pool1(F.relu(self.conv1(x)))
        # Block 2 forward pass
        x = self.pool2(F.relu(self.conv2(x)))
        # Classification head
        x = self.flatten(x)
        x = F.relu(self.fc1(x))
        x = self.fc2(x)
        return x

# Instantiate the model architecture for binary classification
vision_model = TabularCNN(num_classes=2)
print(vision_model)
```

The generated synthetic images stored in `synthetic_dataset/` can be seamlessly loaded via PyTorch’s standard `torchvision.datasets.ImageFolder` class combined with a `DataLoader` loop, optimizing models using typical criteria like `CrossEntropyLoss` or `BCEWithLogitsLoss`.

## Conclusion and Open Horizons

Transforming tabular features into synthetic spatial layouts offers a compelling methodology to bridge classical data problems with state-of-the-art visual architectures. Utilizing **TINTOlib** provides data scientists with a rigorous, reproducible, and standardized framework to systematically test, compare, and scale these transformations while avoiding common pitfalls such as data leakage.

In subsequent entries, we will delve deeper into benchmarking comparative analysis (e.g., non-parametric IGTD vs. parallelized REFINED), evaluating performance shifts when deploying Vision Transformers (ViTs), and rendering feature importance maps through advanced XAI methods.

## References and related publications

The concepts presented in this tutorial are connected to the following research and software publications on TINTO, TINTOlib, tabular-to-image transformation, synthetic spatial representations, hybrid neural networks, and indoor localisation.

### Research articles

1. Jiayun Liu, Manuel Castillo-Cara et al. **Interpretable Hybrid Vision Transformer Architectures for MIMO-Based Indoor Localization using Synthetic Spatial Representations**. *IEEE Internet of Things*. DOI: [10.1109/JIOT.2026.3696106](https://doi.org/10.1109/JIOT.2026.3696106)

2. Jiayun Liu, Manuel Castillo-Cara et al. **A Comprehensive Benchmark of Spatial Encoding Methods for Tabular Data with Deep Neural Networks**. *Information Fusion*. DOI: [10.1016/j.inffus.2025.104088](https://doi.org/10.1016/j.inffus.2025.104088)

3. Manuel Castillo-Cara et al. **MIMO-Based Indoor Localisation with Hybrid Neural Networks**. *IEEE Journal of Selected Topics in Signal Processing*. DOI: [10.1109/JSTSP.2025.3555067](https://doi.org/10.1109/JSTSP.2025.3555067)

4. Reewos Talla-Chumpitaz, Manuel Castillo-Cara et al. **Blurring Image Techniques for Bluetooth-based Indoor Localisation**. *Information Fusion*. DOI: [10.1016/j.inffus.2022.10.011](https://doi.org/10.1016/j.inffus.2022.10.011)

### Software articles

5. Jiayun Liu et al. **TINTOlib: A Python library for transforming tabular data into synthetic images for deep neural networks**. *SoftwareX*. DOI: [10.1016/j.softx.2025.102444](https://doi.org/10.1016/j.softx.2025.102444)

6. Manuel Castillo-Cara et al. **TINTO: Converting Tidy Data into Image for Classification with 2-Dimensional Convolutional Neural Networks**. *SoftwareX*. DOI: [10.1016/j.softx.2023.101391](https://doi.org/10.1016/j.softx.2023.101391)

{% include blog-footer.html %}

