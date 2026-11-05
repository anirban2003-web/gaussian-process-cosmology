# gaussian-process-cosmology
# Gaussian Process Cosmology

This repository contains some of my work with **Gaussian Processes (GPs) for cosmological data analysis**, mainly focused on reconstructing observational residuals and studying their behaviour with redshift.

The notebooks here are practice and internship-related work rather than part of my thesis.

## About Gaussian Processes

A Gaussian Process is a non-parametric way of modelling a function from data. Instead of assuming a particular functional form, the GP describes a distribution over possible functions using a mean function and a covariance kernel.

For cosmological data, this is useful when we want to reconstruct a quantity directly from observations without imposing a specific cosmological model on the reconstruction.

In this project I use GPs to look at residuals in supernova data and obtain a reconstructed mean together with \(1\sigma\) and \(2\sigma\) uncertainty regions.

## GaPP3

The GP calculations make use of **GaPP3**, the Python 3 version of the Gaussian Processes code developed for cosmological applications.

The original methodology is described in:

**Seikel, M., Clarkson, C. & Smith, M. (2012)**  
*Reconstruction of dark energy and expansion dynamics using Gaussian processes*  
JCAP 06 (2012) 036.

DOI: `10.1088/1475-7516/2012/06/036`

GaPP3 repository:  
https://github.com/lighink/GaPP3

GaPP3 is used here as an existing library; the notebooks contain my own applications of the method to the datasets used in this project.

## Data and Analysis

The repository currently contains GP analyses using astronomical data including **Pantheon+** and **DES 5YR** supernova data.

The main things explored are:

- GP reconstruction of observational residuals
- Redshift-dependent behaviour
- GP mean functions
- \(1\sigma\) and \(2\sigma\) uncertainty regions
- Comparison of residuals between different datasets

## Notebooks

### `hubble_GP.ipynb`

Initial exploration of Gaussian Process reconstruction for cosmological data.

### `GP reconstruction residuals (GP).ipynb`

GP reconstruction of observational residuals as a function of redshift.


## Figures

The `figures/` directory contains the main plots generated from the notebooks, including the GP reconstructions and their uncertainty regions.

## Repository structure

```text
gaussian-process-cosmology/
│
├── data/
│   └── datasets used in the analysis
│
├── figures/
│   └── generated figures
│
├── notebooks/
│   ├── GP reconstruction residuals (GP) (DES & Pantheon+).ipynb
│   ├── GP reconstruction residuals (GP).ipynb
│   └── hubble_GP.ipynb
│
└── README.md
```

## Tools

Python · NumPy · Pandas · SciPy · Matplotlib · Jupyter · GaPP3

## Reference

Seikel, M., Clarkson, C. & Smith, M. (2012).  
*Reconstruction of dark energy and expansion dynamics using Gaussian processes.*  
JCAP 06, 036.

https://doi.org/10.1088/1475-7516/2012/06/036

---

**Anirban Mohonta Ayon**  
B.Sc. (Hons.) Physics, Ramjas College, University of Delhi
