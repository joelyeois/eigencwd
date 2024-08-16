# EigenCWD: a spatially varying deconvolution algorithm for single metalens imaging
[Paper]()

[Joel Yeo](https://orcid.org/0000-0001-5160-7628), [Ramon Paniagua-Dominguez](https://orcid.org/0000-0001-7836-681X), [N. Duane Loh](https://orcid.org/0000-0002-8886-510X), [Arseniy Kuznetsov](https://orcid.org/0000-0002-7622-8939)

This repository presents a minimal working example of the eigenCWD algorithm for spatially varying deconvolution for single metalens imaging. The forward blurring model uses the eigenPSF method to decompose the spatially varying PSFs into a linear sum of eigenPSF bases. This decomposition allows for fast computation of spatially varying aberrations such as coma. The eigenCWD utilizes the eigenPSF decomposition to solve the inverse problem of deconvolution using the alternating direction method of multipliers (ADMM) method. This algorithm is a modification from Sroubek's original proposed method based on column-wise decomposition via singular value decomposition (CWD-SVD) [1](https://doi.org/10.1109/LSP.2016.2519764).

## Installation
To run the code, users may first install the required packages listed in the root directory via ```pip install -r requirements.txt```.
After which, the `eigencwd` package can be installed via ```pip install .```.

## Demos
After installation, users may use the demo notebook provided in the `notebooks` folder to run a minimal working example of the eigenCWD algorithm.

## Citation
If you find our work useful in your research, please cite:
```
@article{YEO2024113962,
title = {Ghostbuster: A phase retrieval diffraction tomography algorithm for cryo-EM},
journal = {Ultramicroscopy},
volume = {262},
pages = {113962},
year = {2024},
issn = {0304-3991},
doi = {https://doi.org/10.1016/j.ultramic.2024.113962},
url = {https://www.sciencedirect.com/science/article/pii/S030439912400041X},
author = {Joel Yeo and Benedikt J. Daurer and Dari Kimanius and Deepan Balakrishnan and Tristan Bepler and Yong Zi Tan and N. Duane Loh},
keywords = {Diffraction tomography, Phase retrieval, Cryogenic electron microscopy, Single particle reconstruction, Ewald sphere curvature correction},
}
```

## License
Our code is licensed under GNU GPLv3. By downloading the software, you agree to the terms of this License.
