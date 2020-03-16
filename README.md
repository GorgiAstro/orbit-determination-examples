# Description

This repository provides examples for orbit determination based, in the form of Jupyter Notebooks.

The open-source orbital dynamics library Orekit (https://www.orekit.org/) is used for all calculations, and in particular the Python wrapper developed by [@petrushy](https://github.com/petrushy): https://gitlab.orekit.org/orekit-labs/python-wrapper

# Installation

## Prerequisites
* Anaconda or Miniconda

## Install conda environment

Install the conda environment. For this, you can either import the environment.yml file into Anaconda Navigator, or use the command line
`conda env create -f environment.yml`

If the environment already exists, update it using:
`conda env update -f environment.yml`

## Install Jupyter Lab extensions
### Mandatory extensions
The following extensions are required to use Plotly offline in notebooks:

```
# Enter conda environment
source activate laserod

# Jupyter widgets extension
jupyter labextension install @jupyter-widgets/jupyterlab-manager --no-build

# jupyterlab renderer support
jupyter labextension install jupyterlab-plotly --no-build

# FigureWidget support
jupyter labextension install plotlywidget --no-build

# Build extensions (must be done to activate extensions since --no-build is used above)
jupyter lab build
```

# Use

* Enter conda environment: `source activate orbitdetermination` (or start a terminal directly in the environment using Anaconda Navigator)
* Start Jupyter Lab: `jupyter lab`
* Jupyter Lab should pop up in your browser at the URL http://localhost:8888
