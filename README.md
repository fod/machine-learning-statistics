# Machine Learning and Statistics Assessment Repository

1. [Overview](#overview)
1. [Repository Contents](#repository-contents)
1. [Requirements](#requirements)
1. [How to run](#how-to-run)

## Overview

This repository contains two [Jupyter](https://jupyter.org/) notebooks and ancillary files demonstrating some aspects of data analysis using the Python programming language and various associated technologies in fulfillment of requirements for the *Machine learning and statistics* module of the HDipSc in Computing in Data Analytics at the Galway-Mayo Institute of Technology (GMIT). One notebook, [scikit-learn.ipynb](scikit-learn.ipynb) focuses on the preparation and predictive analysis of data using the Python [scikit-learn](https://scikit-learn.org/stable/) machine learning library. The second, [scipy-stats.ipynb](scipy-stats.ipynb), focuses on performing an ANOVA using the Python statistics library (scipy-stats)[https://docs.scipy.org/doc/scipy/index.html].

## Repository Contents

The repository contains two Jupyter notebooks which are independent of one another;
- [scikit-learn.ipynb](scikit-learn.ipynb) 
- [scipy-stats.ipynb](scipy-stats.ipynb)

The rest of the contents of the repository all support those files in some way. They are:
- README.md; this file
- [requirements.txt](requirements.txt); a list of Python packages required to run the notebooks
- .gitignore; a git support file which may be safely ignored
- [data/](data/); a directory containing two sub directories; penguins/, which contains the penguin data analysed in the [scipy-stats notebook](scipy-stats.ipynb), and wine/, which contains the data used in the [scikit-learn notebook](scikit-learn.ipynb). 

## Requirements

Nothing extra is required to view the contents of repository on [github](https://github.com/fod/fundamentals-data-analysis) or [nbviewer](https://nbviewer.org/) or [binder](https://mybinder.org/). However see [below](#how-to-run) for discussion of the limitations of these formats.

To run these notebooks locally [Python v3.9+](https://www.python.org/) with [Pip](https://pypi.org/project/pip/) or some other package manager is the minimum requirement. In order to clone this repository - the easiest way to acquire the code - [git v.2+](https://git-scm.com/) is required.

Assuming Python is installed then the Python packages listed in [requirements.txt](requirements.txt) are required. These can usually be installed in one go using the [requirements.txt](requirements.txt) file with pip or, presumably, any other Python package manager. See [below](#how-to-run) for details.

## How to run

There are three ways to consume the notebooks in this repository:
1. View here on github by simply clicking on [scikit-learn.ipynb](scikit-learn.ipynb) or [scipy-stats.ipynb](scipy-stats.ipynb), or on [nbviewer](https://nbviewer.org/) by clicking on the appropriate button:

    - For the scikit-learn notebook:&ensp;[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/fod/machine-learning-statistics/blob/main/scikit-learn.ipynb)

    - For the scipy-stats notebook:&ensp;[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/fod/machine-learning-statistics/blob/main/scipy-stats.ipynb)

    This is fine if viewing is all that is required, but if interactivity is necessary or desirable then options 2 or 3 should be considered.

1. View and interact with the notebooks on [binder](https://mybinder.org/) by clicking on the button below:

    [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fod/fundamentals-data-analysis/HEAD)

    This will give access to the entire repository via a [JupyterLab](https://jupyter.org/) session. The code in the notebooks can be changed and executed or new notebooks can be started to experiment with the data, which is, of course, also accessible from the binder session.

1. Clone the repository and run a Jupyter server locally by following these steps (these steps have been tested on a Linux system, some details may differ if using a different operating system):

    - Ensure that [Python v3.9+](https://www.python.org/), [Pip](https://pypi.org/project/pip/), and [git v.2+](https://git-scm.com/) are all installed.
    - Clone the repository by typing git clone git@github.com:fod/machine-learning-statistics.git into a terminal.
    - The repository will be downloaded. When it is complete, enter the machine-learning-statistics directory and create a Python virtual environment in a directory called ```.venv``` with ```python -m venv .venv``` 
    - Activate the virtual environment with ```source .venv/bin/activate```
    - Next install the required packages with ```pip install requirements.txt```
    - Finally, start a jupyter server by typing ```jupyter-lab```. A jupyter lab session should launch in a browser window. If it doesn't, a link which can be pasted into a browser address bar is printed in the terminal.
    
