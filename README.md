# StudyTemplate

This repository provides a comprehensive and modular framework for designing, conducting, and analyzing electroencephalography (EEG) studies. Whether you are a seasoned researcher or a novice in the field of neuroscience, this template aims to streamline the process of setting up EEG experiments, ensuring reproducibility, and facilitating data analysis.

Particular emphasis has been given to:

* Modular design to allow for any study to drop in files straight from the amplifier
* Pre-configured project layouts in accordance with BIDS
* Providing links to training material to improve technical skills
* Constructing visualizations which let researchers explore the data


## Requirements

This project assumes that you are running at least **Python version 3.11**. This can be checked by running the following code snippet inside of an interpreter.

```python
import sys
print(sys.version)
```

This should return a string similar to `3.11.0rc1 (main, Aug 12 2022, 10:02:14) [GCC 11.2.0]`.

If not, follow your platform's instructions for adding new versions of Python.

If you are unable or unfamiliar with this, please contact us or open an issue.

## Skill Prerequisites

The following is a list of must-read materials and course work for users starting their journey from scratch:

1. [Software Carpentry Shell](https://swcarpentry.github.io/shell-novice/)
    * Teaches pathing and commmon terminal use
2. [Software Carpentry Python](https://swcarpentry.github.io/python-novice-inflammation/)
    * Basic Python introduction involving files, plotting, and scripting
3. [BIDS Specification](https://bids-specification.readthedocs.io/en/stable/)
    * Contains the definitions and assumptions for how studies should be layed out
4. [Introduction to Git](https://swcarpentry.github.io/git-novice/)
    * Version control principles and how to download most open source projects
5. [MNE Python](https://mne.tools/stable/index.html)
    * Main platform for interacting with data


## First Steps

To set up the environment, first install Jupyter Lab based on setup instructions from the Python software carpentry linked below.

### Alternative Methods

If you have an alternative installation of Python, (i.e. not Anaconda) you may consider one of the methods in the subsequent paragraphs.

You may also install it via pip with: `pip install jupyterlab`. It can then be launched from the command line via `jupyter lab`. This should produce several lines of text in your terminal. Copy and paste one of the "localhost" URLs into your browser and you should be presented with the standard Jupyter interface.

## Current Notebooks

Below is a list of notebooks in a rough ordering of their intended use.

1. `test_environment`
    * Installs necessary packages and does some basic plotting to verify that things are working
2. `explore_source` 
    * Inspects a bunch of features of a single source recording to determine quality and necessary steps for initialization
3. `init_bids_study`
    * Walks through the steps of building a BIDS study from a list of source files
4. `quick_clean`
    * Performs very basic artifact detection on all bids subjects in the project before saving them to a derivative
5. `erp_study`
    * Based on conditions, performs a traditional ERP study on all subjects in the derivatives


### TODO:

* Test with full data on Windows and Anaconda
    * initial tests are good though!
* Gather feedback
