# Crash Course on [TINTOlib](https://tintolib.readthedocs.io/en/latest/): Tabular Data to Synthetic Images for Vision-Based Machine Learning

[![License](https://img.shields.io/badge/license-Apache%202.0-blue)](https://github.com/oeg-upm/TINTOlib-Documentation/blob/main/LICENSE)  
[![Python Version](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.python.org/pypi/)  
[![Documentation Status](https://readthedocs.org/projects/morph-kgc/badge/?version=latest)](https://tintolib.readthedocs.io/en/latest/)

<div align="center">
  <img src="Images/logo.svg" alt="TINTO Logo" width="150">
</div>

## Overview

## Overview

**TINTOlib** is the first Python library specifically designed to transform tabular data into synthetic images, addressing a critical gap in the integration of tabular and image-based machine learning approaches. Unlike existing tools, **TINTOlib** supports a comprehensive set of transformation techniques optimized for state-of-the-art computer vision models, including Convolutional Neural Networks (CNNs) and Vision Transformers (ViTs). 

This library was introduced and validated in the context of a scientific study, where its methods demonstrated significant improvements in regression and classification tasks when used with hybrid neural network architectures. The study highlighted how TINTOlib bridges the gap between tabular data processing and vision-based deep learning by enabling seamless integration of features extracted from synthetic images with numerical data using hybrid architectures.

Key features of **TINTOlib** include:
- Integration of **state-of-the-art transformation methods** for tabular-to-image conversion, such as IGTD, SuperTML, and REFINED.
- Support for **hybrid architectures** that combine CNNs or ViTs with Multi-Layer Perceptrons (MLPs), leveraging the strengths of both data formats.
- Compatibility with popular frameworks like **TensorFlow** and **PyTorch**, facilitating experimentation and deployment.


## Key Features

- **Data Input Options**:
  - **Pandas DataFrame** for seamless data handling.
  - **CSV Files** following the **Tidy Data** format, where:
    - The last column is the target variable.
    - All other columns are numerical features.
- **Platform Compatibility**: Runs on **Linux**, **Windows**, and **macOS**.
- **Python Versions Supported**: Python 3.7 and above.

## Repository Structure

The repository is organized into the following key sections:

- **Notebooks**: Step-by-step examples for transforming tabular data into images and applying vision models. Includes:
  - **Classification**: Notebooks for classification task.
  - **Regression**: Notebooks for regression task.


## Tabular-to-Image Transformation Methods

All the methods presented can be called using the [TINTOlib](https://tintolib.readthedocs.io/en/latest/) library. The methods presented include:

|                              Model                               |    Class     | Features |                                                                Hyperparameters                                                                 |
|:----------------------------------------------------------------:|:------------:|:--------:|:----------------------------------------------------------------------------------------------------------------------------------------------:|
|            [TINTO](https://github.com/oeg-upm/TINTO)             |  `TINTO()`   |  `blur`  |                   `problem` `algorithm` `pixels` `submatrix` `blur` `amplification` `distance` `steps` `option` `random_seed` `times` `verbose`                   |
|             [IGTD](https://github.com/zhuyitan/igtd)             |   `IGTD()`   |          | `problem` `scale` `fea_dist_method` `image_dist_method` `max_step` `val_step` `error` `switch_t` `min_gain` `zoom` `random_seed` `verbose` |
|       [REFINED](https://github.com/omidbazgirTTU/REFINED)        | `REFINED()`  |          |                                                      `problem` `n_processors` `hcIterations` `zoom` `random_seed` `verbose`      |
|                           [BarGraph]()                           | `BarGraph()`  |          |                                                    `problem` `pixel_width` `gap`  `zoom` `verbose`                                                    |
|                        [DistanceMatrix]()                        | `DistanceMatrix()`  |          |                                                          `problem` `zoom`  `verbose`                                                          |
|                         [Combination]()                          | `Combination()`  |          |                                                             `problem` `zoom`  `verbose`                                                              |
| [SuperTML](https://github.com/GilesStrong/SuperTML_HiggsML_Test) | `SuperTML()` |          |                                             `problem` `columns` `font_size` `image_size` `verbose`                                             |
|                         [FeatureWrap]()                          | `FeatureWrap()`  |          |                                                             `problem` `size` `bins` `zoom` `verbose`                                                              |
|                         [BIE]()                          | `BIE()`  |          |                                                             `problem` `precision` `zoom` `verbose`                                                              |

## More information

- For more detailed information, refer to the **[TINTOlib ReadTheDocs](https://tintolib.readthedocs.io/en/latest/)**.  
- GitHub repository: **[TINTOlib Documentation](https://github.com/oeg-upm/TINTOlib-Documentation)**.
- PyPI: **[PyPI](https://pypi.org/project/TINTOlib/)**.

<!--

## Citation

If you use TINTO in your work, please cite the following:

- **[TINTO: Converting Tidy Data into Images](https://doi.org/10.1016/j.softx.2023.101391)**:
```bib
@article{softwarex_TINTO,
    title = {TINTO: Converting Tidy Data into Image for Classification with 2-Dimensional Convolutional Neural Networks},
    journal = {SoftwareX},
    author = {Manuel Castillo-Cara et al.},
    volume = {22},
    pages = {101391},
    year = {2023},
    doi = {https://doi.org/10.1016/j.softx.2023.101391}
}

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
-->

## License

TINTOlib is available under the **[Apache License 2.0](https://github.com/oeg-upm/TINTOlib-Documentation/blob/main/LICENSE)**.

## Authors
- **[Manuel Castillo-Cara](https://github.com/manwestc) - [manuelcastillo@dia.uned.es](manuelcastillo@dia.uned.es)**
- **[Raúl García-Castro](https://github.com/rgcmme) - [r.garcia@upm.es](r.garcia@upm.es)**
- **[Jiayun Liu](https://github.com/DCY1117) - [jiayun.liu@upm.es](jiayun.liu@upm.es)**
- **[David González Fernández](https://github.com/DavidGonzalezFernandez)**


## Contributors

<div>
<p align = "center">
<kbd><img src="./imgs/logo-oeg.png" alt="Ontology Engineering Group" width="150"></kbd> <kbd><img src="./imgs/logo-upm.png" alt="Universidad Politécnica de Madrid" width="150"></kbd> <kbd><img src="./imgs/logo-uned-.jpg" alt="Universidad Nacional de Educación a Distancia" width="231"></kbd> <kbd><img src="./imgs/logo-uclm.png" alt="Universidad de Castilla-La Mancha" width="115"></kbd> 
</p>
</div>