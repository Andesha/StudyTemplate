# StudyTemplate

A template for running and maintaining an EEG study.

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

## Must Read Material and Skills

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


### TODO:

* Test with full data on Windows and Anaconda
    * initial tests are good though!
* Gather feedback
