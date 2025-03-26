---
title: "TINTOlib - Python library for transforming tabular data into synthetic images"
excerpt: "TINTOlib is an open-source, user-extendable framework that offers new opportunities for users to convert tidy data into images through differents algorithmic methods.<br/><img src='/images/tinto-logo.svg' width='150' align='center' />"
collection: portfolio
category: "Software"
image: "/images/tinto-logo.svg"
---

<div style="text-align: center;">
  <img src="/images/tinto-logo.svg" alt="TINTO Logo" width="200">
</div>

<div style="border: 1px solid #cfd8dc; padding: 1em; margin-bottom: 1.5em; border-radius: 4px; background-color: #f5f8fa;">
  <h2 style="color: #1565c0; text-align: center;">🎉 New Free Course on Udemy! 🎉</h2>
  <p style="text-align: center; font-size: 1em; color: #37474f;">
    We’ve just launched a <strong>100% free course on Udemy</strong> about <strong>using TINTOlib</strong> and developing <strong>Hybrid Neural Networks</strong>.<br/>
    Learn how to turn tabular data into synthetic images and apply CNNs, ViTs, and hybrid architectures like a pro.
  </p>
  <p style="text-align: center;">
    <a href="https://www.udemy.com/course/tintolib-deep-learning-tabutar-data-con-imagenes-sinteticas/?referralCode=16B7C59C2E3B0BD249D0" 
       style="background-color: #1976d2; color: white; padding: 0.7em 1.2em; text-decoration: none; font-weight: bold; border-radius: 5px;">
      👉 Access the Course on Udemy
    </a>
  </p>
</div>

## 🧠 Overview

**TINTOlib** is a powerful Python library that transforms **tidy tabular data** into **synthetic images**, enabling the use of deep learning models like **CNNs** and **Vision Transformers (ViTs)**. This bridges the gap between structured and image-based data for tasks such as classification and regression.

## 📚 Cite TINTOlib

If you use TINTOlib, please cite the following papers:

- [SoftwareX Paper](https://doi.org/10.1016/j.softx.2023.101391):
```bib
@article{softwarex_TINTO,
  title = {TINTO: Converting Tidy Data into Image for Classification with 2-Dimensional Convolutional Neural Networks},
  journal = {SoftwareX},
  author = {Manuel Castillo-Cara and Reewos Talla-Chumpitaz and Raúl García-Castro and Luis Orozco-Barbosa},
  volume={22},
  pages={101391},
  year = {2023},
  issn = {2352-7110},
  doi = {10.1016/j.softx.2023.101391}
}
```
- [INFFUS Paper](https://doi.org/10.1016/j.inffus.2022.10.011):
```bib
@article{inffus_TINTO,
  title = {A novel deep learning approach using blurring image techniques for Bluetooth-based indoor localisation},
  journal = {Information Fusion},
  author = {Reewos Talla-Chumpitaz and Manuel Castillo-Cara and Luis Orozco-Barbosa and Raúl García-Castro},
  volume = {91},
  pages = {173-186},
  year = {2023},
  issn = {1566-2535},
  doi = {10.1016/j.inffus.2022.10.011}
}
```

## 🔧 Features
- Input formats: **CSV** or **Pandas DataFrame**
- Designed for tidy data (target column last)
- Output: grayscale images from reduction and transformation methods
- Compatible with **Linux**, **Windows**, **macOS**
- Requires **Python 3.7+**

## 🧪 Supported Models
Supported image transformation models include:
- TINTO
- IGTD
- REFINED
- BarGraph
- DistanceMatrix
- Combination
- SuperTML
- FeatureWrap
- BIE

Each model has its own hyperparameters and behaviors. See [documentation](https://tintolib.readthedocs.io/en/latest/) for usage.

## 🚀 Getting Started
Install via pip:
```bash
pip install TINTOlib
```
To run examples:
- Use `requirements.txt` for the base environment
- Use `requirements-example.txt` for full deep learning workflows

## 🧩 Example Code
```python
from TINTOlib.tinto import TINTO
model = TINTO(blur=True)
model.fit_transform(data, folder)
```

## 💬 Learn More
- [📘 Documentation](https://tintolib.readthedocs.io/en/latest/)
- [🚀 GitHub](https://github.com/oeg-upm/TINTOlib)
- [📹 Crash Course](https://github.com/oeg-upm/TINTOlib-Crash_Course)

---

## 🎓 License
TINTOlib is released under the **Apache License 2.0**.

## 👥 Authors
- Manuel Castillo-Cara  
- Raúl García-Castro  
- Borja Reinoso  
- David González Fernández  
- Jiayun Liu  

## 🏛️ Institutions
<div style="text-align: center;">
  <img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-oeg.png" alt="Ontology Engineering Group" width="130">
  <img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-upm.png" alt="UPM" width="130">
  <img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-uned-.jpg" alt="UNED" width="130">
  <img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-uclm.png" alt="UCLM" width="130">
</div>

<!-- SEO Structured Data -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "TINTOlib",
  "operatingSystem": "Linux, macOS, Windows",
  "applicationCategory": "Machine Learning Library",
  "description": "TINTOlib is a Python library that converts tabular (tidy) data into synthetic images using various algorithmic methods. It enables the use of CNNs, ViTs and hybrid models with tabular data.",
  "url": "{{ site.url }}{{ page.url }}",
  "image": "{{ site.url }}/images/tinto-logo.svg",
  "softwareVersion": "1.0",
  "author": {
    "@type": "Person",
    "name": "Manuel Castillo-Cara"
  },
  "publisher": {
    "@type": "Organization",
    "name": "Ontology Engineering Group, UPM"
  },
  "license": "https://github.com/oeg-upm/TINTOlib-Documentation/blob/main/LICENSE",
  "downloadUrl": "https://pypi.org/project/TINTOlib/",
  "codeRepository": "https://github.com/oeg-upm/TINTOlib",
  "programmingLanguage": "Python",
  "offers": {
    "@type": "Offer",
    "price": "0.00",
    "priceCurrency": "EUR"
  }
}
</script>