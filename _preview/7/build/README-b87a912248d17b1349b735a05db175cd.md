<p align="center">
  <img style="float: right;" src="https://raw.githubusercontent.com/UXARRAY/uxarray/a6aa6294975f189e8c36dd3d14da745526e53e06/docs/_static/images/logos/uxarray_logo_v_dark.svg" width="110" />
  <img style="float: right;" src="https://easy.gems.dkrz.de/_static/gems.png" width="230" />
  <img style="float: right;" src="https://healpix.sourceforge.io/images/gorski_f1.jpg" width="100" />
</p>

# HEALPix Cookbook

[![nightly-build](https://github.com/ProjectPythia/healpix-cookbook/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/healpix-cookbook/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/healpix-cookbook/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/942299848.svg)](https://zenodo.org/badge/latestdoi/942299848)

This Project Pythia Cookbook covers an introduction to the [**H**ierarchical **E**qual **A**rea iso**L**atitude **Pix**elation (HEALPix)](https://healpix.sourceforge.io/) of the Earth and utilization of 
[easy.gems](https://easy.gems.dkrz.de/index.html#) and [UXarray](https://uxarray.readthedocs.io/) to run data analysis and visualization functionality on HEALPix data sets.

## Motivation

Driven by [The 2025 World Climate Research Programme (WCRP) Digital Earths Global KM-scale Hackathon](https://www.wcrp-esmo.org/activities/wcrp-global-km-scale-hackathon-2025) taking place 12-16 May, a need 
for exploring HEALPix and documenting HEALPix-based workflows that utilize community resources such as the easy.gems documentation and UXarray software tool has emerged. Project Pythia Cookbooks are a great 
medium to publish such documentation in an accessible, reproducible, and citable manner, which can benefit not only the 2025 event but also future collaboration efforts and similar events.

## Authors

[Orhan Eroglu](https://github.com/erogluorhan), [Philip Chmielowiec](https://github.com/philipc2), [Andrew Gettelman](https://github.com/andrewgettelman), [John Clyne](https://github.com/clyne)

### Contributors

<a href="https://github.com/ProjectPythia/healpix-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/healpix-cookbook" />
</a>

## Structure

This cookbook is broken up into a few sections as follows:

### 1. HEALPix Overview

Here, we cover basic information about HEALPix necessary to understand the topics throughout the cookbook 
and provide a lot of links to the resources in order to learn more about HEALPix. 

### 2. easy.gems for HEALPix Analysis & Visualization

This section provides examples of how to load in HEALPix data, use `healpix` package for basic HEALPix 
statistics use `easygems` package's convenience functions to plot the data with matplotlib.

### 3. UXarray for Basic HEALPix Statistics & Visualization

This section walks the reader through loading in and performing basic analysis and visualization on HEALPix 
data using UXarray.

### 4. Advanced UXarray Analysis and Visualization for HEALPix Data

This section will cover advanced UXarray functionality such as remapping, zonal means, cross-sections, etc.

### 5. When to Use Each?

This section is currently under construction, but once complete, we hope to provide some practical guidance 
on what cases either of `easy.gems` or `uxarray` can provide helpful functionality and would be a 
ideal choice.

## Running the Notebooks

You can either run the notebook using [Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html).

Note, not all Cookbook chapters are executable. If you do not see
the rocket ship icon, such as on this page, you are not viewing an
executable book chapter.


### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the `https://github.com/ProjectPythia/healpix-cookbook` repository:

   ```bash
    git clone https://github.com/ProjectPythia/healpix-cookbook.git
   ```

1. Move into the `healpix-cookbook` directory
   ```bash
   cd healpix-cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate healpix-cookbook
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
