---
title: "TINTOlib - Python library for transforming tabular data into synthetic images"
excerpt: "TINTOlib is an open-source, user-extendable framework that offers new opportunities for users to convert tidy data into images through differents algorithmic methods.<br/><img src='/images/tinto-logo.svg' width='150' align='center' />"
collection: portfolio
category: "Software"
image: "/images/tinto-logo.svg"
---


<div>
<p align = "center">
<img src="/images/tinto-logo.svg" alt="TINTO Logo" width="200">
</p>
</div>


<div style="border: 1px solid #cfd8dc; padding: 1em; margin-bottom: 2em; border-radius: 8px; background-color: #f5f8fa;">
  <h2 style="color: #1565c0; text-align: center;">🎉 New Free Course on Udemy! 🎉</h2>
  <p style="text-align: center; font-size: 1.1em; color: #37474f;">
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



<!--
<div>
    <p align = "center">
    <img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo.svg" alt="TINTO Logo" width="150">
    </p>
</div>
-->


**TINTOlib** is a state-of-the-art Python library that transforms **tidy data** (also known as tabular data) into **synthetic images**, enabling the application of advanced deep learning techniques, including **Vision Transformers (ViTs)** and **Convolutional Neural Networks (CNNs)**, to traditionally structured data. This transformation bridges the gap between tabular data and powerful vision-based machine learning models, unlocking new possibilities for tackling regression, classification, and other complex tasks.

**Citing TINTO**: If you used TINTO in your work, please cite the **[SoftwareX](https://doi.org/10.1016/j.softx.2023.101391)**:

```bib
@article{softwarex_TINTO,
    title = {TINTO: Converting Tidy Data into Image for Classification with 2-Dimensional Convolutional Neural Networks},
    journal = {SoftwareX},
    author = {Manuel Castillo-Cara and Reewos Talla-Chumpitaz and Raúl García-Castro and Luis Orozco-Barbosa},
    volume={22},
    pages={101391},
    year = {2023},
    issn = {2352-7110},
    doi = {https://doi.org/10.1016/j.softx.2023.101391}
}
```

And use-case developed in **[INFFUS Paper](https://doi.org/10.1016/j.inffus.2022.10.011)** 

```bib
@article{inffus_TINTO,
    title = {A novel deep learning approach using blurring image techniques for Bluetooth-based indoor localisation},
    journal = {Information Fusion},
    author = {Reewos Talla-Chumpitaz and Manuel Castillo-Cara and Luis Orozco-Barbosa and Raúl García-Castro},
    volume = {91},
    pages = {173-186},
    year = {2023},
    issn = {1566-2535},
    doi = {https://doi.org/10.1016/j.inffus.2022.10.011}
}
```

---

## Features
- Input data formats (2 options):
    - **Pandas Dataframe** 
    - **Files with the following format** 
        - **Tabular files**: The input data must be in **[CSV](https://en.wikipedia.org/wiki/Comma-separated_values)**, taking into account the **[Tidy Data](https://www.jstatsoft.org/article/view/v059i10)** format.
        - **Tidy Data**: The **target** (variable to be predicted) should be set as the last column of the dataset. Therefore, the first columns will be the features.
        - All data must be in numerical form.
        
- Runs on **Linux**, **Windows** and **macOS** systems.
- Compatible with **[Python](https://www.python.org/)** 3.7 or higher.

---

## Models
TINTOlib includes a variety of models for generating synthetic images. Below is a summary of the supported models and their hyperparameters:

| Models | Class | Hyperparameters |
|:----------------------------------------------------------------:|:------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| [TINTO](https://github.com/oeg-upm/TINTO) | `TINTO()` | `problem` `normalize` `verbose` `pixels` `algorithm` `blur` `submatrix` `amplification` `distance` `steps` `option` `times` `train_m` `zoom` `random_seed` |
| [IGTD](https://github.com/zhuyitan/igtd) | `IGTD()` | `problem` `normalize` `verbose` `scale` `fea_dist_method` `image_dist_method` `error` `max_step` `val_step` `switch_t` `min_gain` `zoom` `random_seed` |
| [REFINED](https://github.com/omidbazgirTTU/REFINED) | `REFINED()` | `problem` `normalize` `verbose` `hcIterations` `n_processors` `zoom` `random_seed` |
| [BarGraph](https://github.com/anuraganands/Non-image-data-classification-with-CNN/) | `BarGraph()` | `problem` `normalize` `verbose` `pixel_width` `gap` `zoom` |
| [DistanceMatrix](https://github.com/anuraganands/Non-image-data-classification-with-CNN/) | `DistanceMatrix()` | `problem` `normalize` `verbose` `zoom` |
| [Combination](https://github.com/anuraganands/Non-image-data-classification-with-CNN/) | `Combination()` | `problem` `normalize` `verbose` `zoom` |
| [SuperTML](https://github.com/GilesStrong/SuperTML_HiggsML_Test) | `SuperTML()` | `problem` `normalize` `verbose` `pixels` `feature_importance` `font_size` `random_seed` |
| [FeatureWrap](https://link.springer.com/chapter/10.1007/978-3-319-70139-4_87) | `FeatureWrap()` | `problem` `normalize` `verbose` `size` `bins` `zoom` |
| [BIE](https://ieeexplore.ieee.org/document/10278393) | `BIE()` | `problem` `normalize` `verbose` `precision` `zoom` |

---

## Getting Started

**You can install TINTOlib using [Pypi](https://pypi.org/project/TINTOlib/)**:

```
    pip install TINTOlib
```

TINTOlib already includes all necessary dependencies, so there’s no need to install them individually.

However, if you prefer manual installation or want to explore the full environment:

- The repository includes a `requirements.txt` file listing the **core dependencies** required to use TINTOlib. You can directly run the **TINTOlib-example.ipynb** notebook located in the examples/ folder using the dependencies listed in `requirements.txt`.
- **Other notebooks**, which include training deep learning models on the generated images, require additional libraries. To run them, install the extended dependencies from `requirements-example.txt`:

---

### Importing a Specific Model

To use a specific image transformation model, import it directly. For example, to use **TINTO**:

```python
from TINTOlib.tinto import TINTO
```

To import a specific model use 
``` python
    from TINTOlib.tinto import TINTO
```

Create the model. If you don't set any hyperparameter, the model will use the default values, refer to the **[Models Section](#models)** or the **[TINTO Documentation](https://tintolib.readthedocs.io/en/latest/)**.

```python
    model = TINTO(blur=True)
```

### Generating Synthetic Images
To generate synthetic images, use the following workflow with the `fit`, `transform`, and `fit_transform` methods:

#### **Fitting the Model**
The `fit` method trains the model on the tabular data and prepares it for image generation.

```python
model.fit(data)
```

#### **Generating Synthetic Images**
The `transform` method generates and saves synthetic images in a specified folder. It requires the model to be fitted first.

```python
model.transform(data, folder)
```


#### **Combining Fit and Transform**
The `fit_transform` method combines the training and image generation steps. It fits the model to the data and generates synthetic images in one step.

```python
model.fit_transform(data, folder)
```


#### Notes:
- **The model must be fitted** before using the `transform` method. If the model isn't fitted, a `RuntimeError` will be raised.

---

## Documentation

For detailed usage, examples, and tutorials, visit the **[TINTOlib Documentation](https://tintolib.readthedocs.io/en/latest/)**.

## How to use TINTOlib - Google Colab crash course
To get started with **TINTOlib**, a dedicated **[crash course repository](https://github.com/oeg-upm/TINTOlib-Crash_Course)** is available. This repository provides a comprehensive guide to using TINTOlib for transforming tabular data into synthetic images and applying these images to machine learning tasks. It includes:

- **Slides and Jupyter notebooks** demonstrating how to:
  - Transform tabular data into images using **TINTOlib**.
  - Apply state-of-the-art vision models like **Vision Transformers (ViTs)** and **Convolutional Neural Networks (CNNs)** to classification and regression problems.

- Integration of **Hybrid Neural Networks (HyNNs)**, where:
  - **One branch** (MLP) processes the original tabular data.
  - **Another branch** (CNN or ViT) processes synthetic images.

This architecture leverages the strengths of both tabular and image-based data representations, enabling improved performance on complex machine learning tasks. The repository is ideal for those looking to integrate image-based deep learning techniques into tabular data workflows.
## Converting Tidy Data into image

For example, the following table shows a classic example of the [IRIS CSV dataset](https://archive.ics.uci.edu/ml/datasets/iris) as it should look like for the run:


| sepal length | sepal width | petal length | petal width | target |
|--------------|-------------|--------------|-------------|--------|
| 4.9 | 3.0 | 1.4 | 0.2 | 1 |
| 7.0 | 3.2 | 4.7 | 1.4 | 2 |
| 6.3 | 3.3 | 6.0 | 2.5 | 3 |


### Simple example with TINTO Method


<div>
<p align = "center">
<kbd><img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/blurring.png" alt="TINTO blurring" width="250"></kbd>
</p>
</div>

---

## License

TINTOlib is available under the **[Apache License 2.0](https://github.com/oeg-upm/TINTOlib-Documentation/blob/main/LICENSE)**.

## Authors
- **[Manuel Castillo-Cara](https://github.com/manwestc)**
- **[Raúl García-Castro](https://github.com/rgcmme)**
- **[Borja Reinoso](https://github.com/borjarei)**
- **[David González Fernández](https://github.com/DavidGonzalezFernandez)**
- **[Jiayun Liu](https://github.com/DCY1117)**


## Contributors

<div>
<p align = "center">
<kbd><img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-oeg.png" alt="Ontology Engineering Group" width="150"></kbd> <kbd><img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-upm.png" alt="Universidad Politécnica de Madrid" width="150"></kbd> <kbd><img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-uned-.jpg" alt="Universidad Nacional de Educación a Distancia" width="231"></kbd> <kbd><img src="https://raw.githubusercontent.com/DCY1117/TEMP-Images/refs/heads/main/TINTOlib-images/logo-uclm.png" alt="Universidad de Castilla-La Mancha" width="115"></kbd> 
</p>
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