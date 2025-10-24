# Bayesian-Analysis-With-Python

This repository is prepared for personal study purposes only. It is not intended as a book, publication, or commercial product. These are my personal study notes. The content includes information compiled from various sources and is used solely for educational and research purposes. If you believe any material violates copyright, please contact me and I will make the necessary adjustments.

## Setup

**PyMC** ıs a powerful probabilistic programming framework for Bayesian analysis in Python.  
Conda-based setup with **Miniforge** ıs recommended. (I also had issues with pip package manager on my computer to use PyMC.)

### Miniforge

Miniforge is a minimal, community-driven conda installer that uses the `conda-forge` channel by default. It offers several advantages:

- Fully open source
- Lightweight: installs only essential packages
- Seamless compatibility with `conda-forge` packages like PyMC

### Preparing the Environment

Download the appropriate installer for your operating system from the official GitHub page:

https://github.com/conda-forge/miniforge

After installation, open your Miniforge Terminal and check your current Conda environments:

```bash
conda env list
```

If you've just installed Miniforge, you should primarily see the (base) environment listed.

Create a new Conda environment named `bayesian` and install all the necessary libraries:

```bash
conda create -n bayesian pymc arviz numpy scipy pandas matplotlib seaborn jupyterlab ipykernel ipywidgets -c conda-forge
```

Once the environment is created, activate it:

```bash
conda activate bayesian
```

Check the details of your activated environment:

```bash
conda info
```

See all the packages installed within `bayesian` environment:

```bash
conda list
```

Install a package later:

```bash
conda install scikit-learn -c conda-forge
```

Deactivate or delete environment:

```bash
conda deactivate
```

```bash
conda env remove -n bayesian
```
