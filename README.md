Memory Systems Lab iPosition Data Pipeline
==========================================

This data pipeline is meant for the processing of iPosition data. It will output all the pre-2017 metrics as well as the newer metrics. It has a large number of options which will be enumerated in this readme. It can really run on any spatial/temporal reconstruction data whose outputs are formatted properly (TSV).

Install
-------

Install Git: https://git-scm.com/downloads if you don't already have it.

Install Anaconda Python: https://www.continuum.io/downloads if you don't already have it.

In a command prompt/terminal (you may need to run as administrator), navigate to/create an **empty directory**, then run:

    conda create -n iposition python=2.7 --yes
    
    activate iposition
    
    conda install scipy jupyter scikit-learn --yes
    
    git clone https://github.com/kevroy314/msl-iposition-pipeline/ .
    
    pip install .
    

Updating
--------

To update the script to the latest version navigate to/create an **empty directory**, then run:

    activate iposition
    
    git clone https://github.com/kevroy314/msl-iposition-pipeline/ .
    
    pip install --upgrade .
    

If you'd like to update without changing the dependencies you can instead, from an **empty directory**, run:


    activate iposition
    
    git clone https://github.com/kevroy314/msl-iposition-pipeline/ .
    
    pip install --upgrade . --no-deps
    

Usage
-----

Note: this section is incomplete and will be updated as new features are added.

Although there are many ways to interface with this analysis software, the easiest is to use a Jupyter Notebook in your web browser. To begin, navigate to wherever you downloaded the github repository (from the installation steps), and open a command prompt/terminal window. Then run:

    activate iposition
    
    jupyter notebook
    

A window in your default web browser (preferrably Chrome) will open with a listing of the files and subdirectories in that github repository directory. Click on the 'tests' folder. This folder contains a variety of interactive scripts to perform various functions using the software package. To run a simple analysis on a directory of data, generating an output CSV, click Pipeline-Test.ipynb. This will open a new window in which there are cells containing code as well as additional documentation.

To run the simple analysis, scroll down to Batch Pipeline Test and select the first code cell. Press Shift+Enter and you will see the cell execute (the first cell imports the software). Click Shift+Enter again and wait. A popup asking you to select a folder will appear. Select your data folder and click OK. The data will be processed and a CSV file will be created locally in the 'tests' folder. 

If you want to run with different settings/paramters, see the documentation for the batch_pipeline function here: http://msl-iposition-pipeline.readthedocs.io/en/latest/source/cogrecon.core.html#module-cogrecon.core.batch_pipeline

In particular, note if you have trial_by_trial_accuracy set to True or False (to determine if accuracy is computer within or across trials) and if you need actual_coordinate_prefixes set to True or False (if you have an actual_coordinates.txt file for every participant).

Output
--------

| Column Name | Description |
| ---      | ---       |
| subID | placeholder |
| trial | placeholder |
| Original Misplacement | placeholder |
| Original Swap | placeholder |
| Original Edge Resizing | placeholder |
| Original Edge Distortion | placeholder |
| Axis Swap Pairs | placeholder |
| Pre-Processed Accurate Placements | placeholder |
| Pre-Processed Inaccurate Placements | placeholder |
| Pre-Processed Accuracy Threshold | placeholder |
| Deanonymized Accurate Placements | placeholder |
| Deanonymized Inaccurate Placements | placeholder |
| Deanonymized Accuracy Threshold | placeholder |
| Raw Deanonymized Misplacement | placeholder |
| Post-Deanonymized Misplacement | placeholder |
| Transformation Auto-Exclusion | placeholder |
| Number of Points Excluded From Geometric Transform | placeholder |
| Rotation Theta | placeholder |
| Scaling | placeholder |
| Translation Magnitude | placeholder |
| Translation | placeholder |
| TranslationX | placeholder |
| TranslationY | placeholder |
| Geometric Distance Threshold | placeholder |
| Post-Transform Misplacement | placeholder |
| Number of Components | placeholder |
| Accurate Single-Item Placements | placeholder |
| Inaccurate Single-Item Placements | placeholder |
| True Swaps | placeholder |
| Partial Swaps | placeholder |
| Cycle Swaps | placeholder |
| Partial Cycle Swaps | placeholder |
| Misassignment | placeholder |
| Accurate Misassignment | placeholder |
| Inaccurate Misassignment | placeholder |
| Swap Distance Threshold | placeholder |
| True Swap Data Distance | placeholder |
| True Swap Actual Distance | placeholder |
| Partial Swap Data Distance | placeholder |
| Partial Swap Actual Distance | placeholder |
| Cycle Swap Data Distance | placeholder |
| Cycle Swap Actual Distance | placeholder |
| Partial Cycle Swap Data Distance | placeholder |
| Partial Cycle Swap Actual Distance | placeholder |
| Unique Components | placeholder |
| Contains Category Data | placeholder |
| Category Label | placeholder |
| Accurate Misassignment Pairs | placeholder |
| Inaccurate Misassignment Pairs | placeholder |
| num_rows_with_nan| | placeholder |
