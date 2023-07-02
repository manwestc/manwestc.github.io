---
title: "Software: TINTOlib - Python library for transforming tabular data into images with 2-Dimensional Convolutional Neural Networks"
excerpt: "TINTOlib is an open-source, user-extendable framework that offers new opportunities for users to convert tidy data into images through differents algorithmic methods.<br/><img src='/images/tinto-logo.svg' width='150' align='center' />"
collection: portfolio
---


<div>
<p align = "center">
<img src="/images/tinto-logo.svg" alt="TINTO Logo" width="200">
</p>
</div>


## Abstract
[TINTOlib](https://github.com/oeg-upm/TINTOlib){:target="_blank"} is a state-of-the-art library that wraps the most important techniques for the construction of Synthetic Images from Sorted Data (also known as Tabular Data).

**Citing TINTO**: If you used TINTOlib in your work, please cite the **[INFFUS Paper](https://github.com/oeg-upm/TINTO){:target="_blank"}**:

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

You can find all the documentation and sources of TINTOlib in [Read the Docs](https://tintolib.readthedocs.io/en/latest/){:target="_blank"}.

<!--
## Video Example

<div>
<p style = 'text-align:center;'>
<iframe width="500" height = "320"
src="https://user-images.githubusercontent.com/102165947/212918739-89fca790-3360-4a8c-89b7-443f294fba6f.mp4">
</iframe>
</p>
</div>
-->

## Main Features

- TINTOlib use seven different state-of-art methods: [TINTO](https://tintolib.readthedocs.io/en/latest/tinto.html){:target="_blank"}, [IGTD](https://tintolib.readthedocs.io/en/latest/igtd.html){:target="_blank"}, [Refined](https://tintolib.readthedocs.io/en/latest/refined.html){:target="_blank"}, [SuperTML](https://tintolib.readthedocs.io/en/latest/supertml.html){:target="_blank"}, [DistanceMatrix](https://tintolib.readthedocs.io/en/latest/distancematrix.html){:target="_blank"}, [BarGraph](https://tintolib.readthedocs.io/en/latest/bargraph.html){:target="_blank"} and [Combination](https://tintolib.readthedocs.io/en/latest/combination.html){:target="_blank"}.
- Supports all CSV data in **[Tidy Data](https://www.jstatsoft.org/article/view/v059i10){:target="_blank"}** format.
- For now, the algorithm converts tabular data for regression and classification problems into machine learning.
- Input data formats:
    - **Tabular files**: The input data must be in **[CSV](https://en.wikipedia.org/wiki/Comma-separated_values){:target="_blank"}**, taking into account the **[Tidy Data](https://www.jstatsoft.org/article/view/v059i10){:target="_blank"}** format.
    - **Tidy Data**: The **target** (variable to be predicted) should be set as the last column of the dataset. Therefore, the first columns will be the features.
    - All data must be in numerical form. TINTOlib does not accept data in string or any other non-numeric format.
- Depends on the method, the synthetic images to be created will be in black and white, i.e. in 1-channel, o RGB, i.e., 3-channel.
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


