---
title: "Software: TINTO - Converting Tidy Data into Image for Classification with 2-Dimensional Convolutional Neural Networks"
excerpt: "TINTO is an open-source, user-extendable framework that offers new opportunities for users to convert tidy data into images through the representation of characteristic pixels.<br/><img src='/images/tinto-logo.svg' width='150' align='center' />"
collection: portfolio
category: "Software"
---


<div>
<p align = "center">
<img src="/images/tinto-logo.svg" alt="TINTO Logo" width="200">
</p>
</div>

<div style="border: 2px solid #4CAF50; padding: 1em; margin-bottom: 2em; border-radius: 8px; background-color: #f9fff9;">
  <h2 style="color: #2e7d32; text-align: center;">🎉 New Free Course on Udemy! 🎉</h2>
  <p style="text-align: center; font-size: 1.1em;">
    We’ve just launched a <strong>100% free course on Udemy</strong> about <strong>using TINTOlib</strong> and developing <strong>Hybrid Neural Networks</strong>.<br/>
    Learn how to turn tabular data into synthetic images and apply CNNs, ViTs, and hybrid architectures like a pro.
  </p>
  <p style="text-align: center;">
    <a href="https://www.udemy.com/course/tintolib-deep-learning-tabutar-data-con-imagenes-sinteticas/?referralCode=16B7C59C2E3B0BD249D0" 
       style="background-color: #4CAF50; color: white; padding: 0.7em 1.2em; text-decoration: none; font-weight: bold; border-radius: 5px;">
      👉 Access the Course on Udemy
    </a>
  </p>
</div>


## Abstract
[TINTO](https://github.com/oeg-upm/TINTO){:target="_blank"} is an open-source, user-extendable framework that offers new opportunities for users to convert tidy data into images through the representation of characteristic pixels. For this transformation, TINTO implemented two-dimensional reduction algorithms, such as PCA and t-SNE. Our proposal also includes a technique used in painting known as blurring, which adds more ordered information to the image and can improve the classification task in CNNs.

<div>
<p style = 'text-align:center;' width='200'>
<img src='/images/tinto-framework.png'>
</p>
</div>

**Citing TINTO**: If you used TINTO in your work, please cite the **[INFFUS Paper](https://doi.org/10.1016/j.inffus.2022.10.011){:target="_blank"}**:

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

And the **[SoftwareX paper](https://doi.org/10.1016/j.softx.2023.101391){:target="_blank"}**

```bib
@article{softwarex_TINTO,
    title = {TINTO: Converting Tidy Data into Image for Classification with 2-Dimensional Convolutional Neural Networks},
    journal = {SoftwareX},
    author = {Manuel Castillo-Cara and Reewos Talla-Chumpitaz and Raúl García-Castro and Luis Orozco-Barbosa},
    year = {2023},
    issn = {2352-7110},
    volume = {22},
    pages = {101391},
    doi = {https://doi.org/10.1016/j.softx.2023.1013911}
}
```

## Documentation

You can find all the documentation and sources of TINTO in [OEG GitHub](https://github.com/oeg-upm/TINTO){:target="_blank"}.

## Video Example

<div>
<p style = 'text-align:center;'>
<iframe width="500" height = "320"
src="https://user-images.githubusercontent.com/102165947/212918739-89fca790-3360-4a8c-89b7-443f294fba6f.mp4">
</iframe>
</p>
</div>

## Main Features

- Supports all CSV data in **[Tidy Data](https://www.jstatsoft.org/article/view/v059i10){:target="_blank"}** format.
- For now, the algorithm converts tabular data for binary and multi-class classification problems into machine learning.
- Input data formats:
    - **Tabular files**: The input data must be in **[CSV](https://en.wikipedia.org/wiki/Comma-separated_values){:target="_blank"}**, taking into account the **[Tidy Data](https://www.jstatsoft.org/article/view/v059i10){:target="_blank"}** format.
    - **Tidy Data**: The **target** (variable to be predicted) should be set as the last column of the dataset. Therefore, the first columns will be the features.
    - All data must be in numerical form. TINTO does not accept data in string or any other non-numeric format.
- Two dimensionality reduction algorithms are used in image creation, **[PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html#sklearn.decomposition.PCA){:target="_blank"}** and **[*t*-SNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html){:target="_blank"}** from the Scikit-learn Python library.
- The synthetic images to be created will be in black and white, i.e. in 1 channel.
- The synthetic image **dimensions** can be set as a parameter when creating them.
- The synthetic images can be created using **characteristic pixels** or **blurring** painting technique (expressing an overlap of pixels as the **maximum** or **average**).
- Runs on **Linux**, **Windows** and **macOS** systems.
- Compatible with **[Python](https://www.python.org/){:target="_blank"}** 3.7 or higher.

## Input
The following table shows a classic example of the [IRIS CSV dataset](https://archive.ics.uci.edu/ml/datasets/iris){:target="_blank"} as it should look like for the run:

| sepal length | sepal width | petal length | petal width | target |
|--------------|-------------|--------------|-------------|--------|
| 4.9          | 3.0         | 1.4          | 0.2         | 1      |
| 7.0          | 3.2         | 4.7          | 1.4         | 2      |
| 6.3          | 3.3         | 6.0          | 2.5         | 3      |

## Output
The following Figure show the output of TINTO:

<div>
<p style = 'text-align:center;'>
<img src='/images/tinto1.png'>
</p>
</div>

<!-- SEO Structured Data -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "TINTO",
  "operatingSystem": "Linux, macOS, Windows",
  "applicationCategory": "Machine Learning Library",
  "description": "TINTO is an open-source Python framework that transforms tabular (tidy) data into black-and-white images using PCA, t-SNE and blurring techniques. It is compatible with CNN-based classification tasks.",
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
  "license": "https://github.com/oeg-upm/TINTO/blob/main/LICENSE",
  "codeRepository": "https://github.com/oeg-upm/TINTO",
  "programmingLanguage": "Python",
  "offers": {
    "@type": "Offer",
    "price": "0.00",
    "priceCurrency": "EUR"
  }
}
</script>

