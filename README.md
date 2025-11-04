# Optimising quantitative methods to assess the efficacy of clearing protocols for light-sheet microscopy - Jupyter Notebooks

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FrancisCrickInstitute/CALM_Template/HEAD?labpath=blob%2Fmain%2Fsegment_image.ipynb)
[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3115/)
![Commit activity](https://img.shields.io/github/commit-activity/y/FrancisCrickInstitute/CALM_Template?style=plastic)
![GitHub](https://img.shields.io/github/license/FrancisCrickInstitute/CALM_Template?color=green&style=plastic)

## Overview
This code is written for the 2025 Crick BioImage Analsyis Symposium (CBIAS) as a method of data analysis for the poster **'Optimising quantitative methods to assess the efficacy of clearing protocols for light-sheet microscopy'**. In this code, our aim is to provide a quick, user-friendly pipeline to assess clearing efficacy of a 3-dimensional sample using simple statistical parameters, broadening scientific communication and easing access for those without computational expertise.

![screenshot](https://github.com/dbekat/CBIAS25_clearing_efficacy_code/blob/resource_add/resources/CBIAS%20Logo.png)


## Content
This repo contains 2 Jupyter Notebooks:

- `pixel_intensity_measurement.ipynb`: a Notebook which imports an image and measures the properties of the image to assess clearing efficacy, and saves this data to a `.csv` file.
- `combine_csv.ipynb`: a Notebook which combines several of these `.csv` files to combine data and visualise your data into a lineplot to compare/contrast, which can then be saved and used.

This repo will also have example data (`test_image.tif`), on which these notebooks can be used and tested for modifications. 


## Contact info

If you have any questions regarding this work or any suggestions, please feel free to reach out:

>Deniz Bekat - *deniz.bekat@crick.ac.uk*

>Alessandro Ciccarelli - *alessandro.ciccarelli@crick.ac.uk*

>David Barry - *david.barry@crick.ac.uk*

## How To Run the Code in This Repo

A step-by-step guide is presented below. **You only need to perform steps 1 and 2 once.** Every subsequent time you want to run the code, skip straight to step 3.

### Step 1
#### Install a Python Distribution

We recommend using conda as it's relatively straightforward and makes the management of different Python environments simple. You can install conda from [here](https://conda.io/projects/conda/en/latest/user-guide/install/index.html#regular-installation) (miniconda will suffice).

### Step 2
#### Set Up Environment

Once conda is installed, open a terminal (Mac) or command line (Windows) and run the following series of commands:

```
conda create --name calm_env pip python=3.11.9
conda activate calm_template
python -m pip install -r <path to this repo>/requirements.txt
```
where you need to replace `<path to this repo>` with the location on your file system where you downloaded this repo. You will be presented with a list of packages to be downloaded and installed. The following prompt will appear:
```
Proceed ([y]/n)?
```
Hit Enter and all necessary packages will be downloaded and installed - this may take some time. When complete, you can deactivate the environment you have created with the following command.

```
conda deactivate
```
You have successfully set up an environment!

### Step 3
#### Open the notebook

The following commands will launch a Jupyter notebook:
```
conda activate calm_env
jupyter notebook <path to this repo>/pixel_intensity_measurement.ipynb
```

The Jupyter Notebook should open in your browser - follow the step-by-step instructions in the notebook to run the code. If you are not familiar with Jupyter Notebooks, you can find a detailed introduction [here](https://jupyter-notebook.readthedocs.io/en/latest/notebook.html#introduction).

### (Optional) Step 4
#### Set up your repo to run on Binder

[Binder](https://mybinder.org/) is a really nice way to allow people to run your Jupyter notebooks directly from GitHub - just [follow this handy guide from the Turing Institute](https://the-turing-way.netlify.app/communication/binder/zero-to-binder.html) to get your repo set up. To run the code in this template repo on Binder, click [here](https://mybinder.org/v2/gh/FrancisCrickInstitute/CALM_Template/HEAD?labpath=blob%2Fmain%2Fsegment_image.ipynb).
