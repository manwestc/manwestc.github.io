---
title: "TINTO: Software to convert Tidy Data into Images"
excerpt: "TINTO is an open-source, user-extendable framework that offers new opportunities for users to convert tidy data into images through the representation of characteristic pixels.<br/><img src='/images/tinto1.png' width='320' height='300' align='center' />"
collection: portfolio
---

## Abstract
[TINTO](https://doi.org/10.1016/j.inffus.2022.10.011) is an open-source, user-extendable framework that offers new opportunities for users to convert tidy data into images through the representation of characteristic pixels. For this transformation, TINTO implemented two-dimensional reduction algorithms, such as PCA and t-SNE. Our proposal also includes a technique used in painting known as blurring, which adds more ordered information to the image and can improve the classification task in CNNs.

**Citing TINTO**: If you used TINTO in your work, please cite the **[INFFUS Paper](https://doi.org/10.1016/j.inffus.2022.10.011)**:

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

## Documentation

You can find all the documentation and sources of TINTO in [OEG GitHub](https://github.com/oeg-upm/TINTO)

## Video Example

<div>
<p style = 'text-align:center;'>
<iframe width="500" height = "320"
src="https://user-images.githubusercontent.com/102165947/212918739-89fca790-3360-4a8c-89b7-443f294fba6f.mp4">
</iframe>
</p>
</div>

## Main Features

- Supports all CSV data in **[Tidy Data](https://www.jstatsoft.org/article/view/v059i10)** format.
- For now, the algorithm converts tabular data for binary and multi-class classification problems into machine learning.
- Input data formats:
    - **Tabular files**: The input data must be in **[CSV](https://en.wikipedia.org/wiki/Comma-separated_values)**, taking into account the **[Tidy Data](https://www.jstatsoft.org/article/view/v059i10)** format.
    - **Tidy Data**: The **target** (variable to be predicted) should be set as the last column of the dataset. Therefore, the first columns will be the features.
    - All data must be in numerical form. TINTO does not accept data in string or any other non-numeric format.
- Two dimensionality reduction algorithms are used in image creation, **[PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html#sklearn.decomposition.PCA)** and **[*t*-SNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)** from the Scikit-learn Python library.
- The synthetic images to be created will be in black and white, i.e. in 1 channel.
- The synthetic image **dimensions** can be set as a parameter when creating them.
- The synthetic images can be created using **characteristic pixels** or **blurring** painting technique (expressing an overlap of pixels as the **maximum** or **average**).
- Runs on **Linux**, **Windows** and **macOS** systems.
- Compatible with **[Python](https://www.python.org/)** 3.7 or higher.

## Input
The following table shows a classic example of the [IRIS CSV dataset](https://archive.ics.uci.edu/ml/datasets/iris) as it should look like for the run:

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
