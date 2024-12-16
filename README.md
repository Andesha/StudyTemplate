# EEGStudyFlow - A template for EEG analyses

This repository provides a comprehensive and modular framework for designing, conducting, and analyzing electroencephalography (EEG) studies. Whether you are a seasoned researcher or a novice in the field of neuroscience, this template aims to streamline the process of setting up EEG experiments, ensuring reproducibility, and facilitating data analysis.

Particular emphasis has been given to:

* Modular design to allow for any study to drop in files straight from the amplifier
* Pre-configured project layouts in accordance with [BIDS](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/electroencephalography.html)
* Providing links to training material to improve technical skills
* Constructing visualizations which let researchers explore the data

## Prerequisites
### EEG Fundamentals

If you are brand new to EEG analysis and are seeking the fundamentals from a theoretical standpoint it is suggested to start with the following list:

* [Learning EEG: a self-guided course and atlas](https://www.learningeeg.com)
* [Virtual ERP Boot Camp: Introduction to ERPs](https://courses.erpinfo.org/courses/Intro-to-ERPs)
* [EEG resources at the INCF Training Space](https://training.incf.org/topic-wise-search?filter=eeg)

### Technical Skills

The following is a list of must-read materials and course work for users starting their journey from scratch:

1. [Software Carpentry Shell](https://swcarpentry.github.io/shell-novice/) teaches the rudiments of terminal use and command line interfaces
2. [Software Carpentry Python](https://swcarpentry.github.io/python-novice-inflammation/) provides a basic Python introduction involving files, plotting, and scripting
3. [BIDS Specification](https://bids-specification.readthedocs.io/en/stable/) contains the definitions and assumptions for how studies should be laid out
4. [Introduction to Git](https://swcarpentry.github.io/git-novice/) introduces version control principles and how to download most open source projects
5. [MNE Python](https://mne.tools/stable/index.html) is a platform for interacting with data

## Requirements for running the content of this analysis template

If you are new to command line environments, it is strongly recommended that your familiarize yourself with first tutorial in above list, "[Technical Skill Prerequisites](#technical-skill-prerequisites)". It will make your life a lot easier.

### Python
This project assumes that you are running at least **Python version 3.11**. This can be checked by running the following code snippet inside of an interpreter.

```python
import sys
print(sys.version)
```

This should return a string similar to `3.11.0rc1 (main, Aug 12 2022, 10:02:14) [GCC 11.2.0]`.

If not, follow your platform's instructions for adding new versions of Python. If you are unable or unfamiliar with this, please contact us or open an issue.

### Jupyter Lab

Install Jupyter Lab by following the setup instructions from the Python software carpentry linked in this document ("2" in the above list of "[Technical Skill Prerequisites](#technical-skill-prerequisites)").

#### Alternate installation methods for Jupyter Lab

Another popular way of installing Python uses the "pip" Python package manager:

```pip install jupyterlab```

On many systems, the command in question is in fact `pip3`, and so the installation command would be:

```pip3 install jupyterlab```

### Clone this repo locally

To make a local copy of this repository, use the `git` command from your Terminal app:

```git clone https://github.com/Andesha/StudyTemplate.git```

### Running the notebooks

Once Jupyter Lab is installed and you have cloned the repository, the easiest is to change directory into "StudyTemplate" and launching Jupyter Lab from there. So, assuming you are in the directory where ran the git cloning command above:

        cd StudyTemplate
        jupyter-lab

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

* Provide some sort of graphic for skills hierarchy
* Provide some sort of graphic for notebook flow


## Acknowledgements 
This work has been supported by **[EEGNet.org](https://eegnet.org)** and Brain Canada, in partnership with Brock University, Laval-CERVO and the McGill Centre for Integrative Neuroscience ([MCIN](https://mcin.ca)). 
Thanks also to the **Canadian Open Neuroscience Platform** [CONP.ca](https://conp.ca) for additional guidance
