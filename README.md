# PyCTRSA

[![PyPI version](https://img.shields.io/pypi/v/pyctrsa?style=flat-square)](https://pypi.org/project/pyctrsa/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

#### A Python toolbox for Cross-Temporal Representation Similarity Analysis (RSA)-based Decoding on EEG/MEG data

## Download
> pip install pyctrsa

## Citation

Lu, Zitong. (2020, November 14). PyCTRSA: A Python package for cross-temporal representational similarity analysis-based E/MEG decoding (Version 0.1.0). Zenodo. http://doi.org/10.5281/zenodo.4273674

## Required Dependencies

- **[Numpy](https://www.numpy.org)**: a fundamental package for scientific computing.
- **[SciPy](https://www.scipy.org/scipylib/index.html)**: a package that provides many user-friendly and efficient numerical routines.
- **[Matplotlib](https://matplotlib.org)**: a Python 2D plotting library.
- **[NeuroRA](https://zitonglu1996.github.io/NeuroRA/)**: a Python toolbox for multimode neural data Representation Analysis.

## Hightlight
In traditional RSA, we can only use a coding model RDM to fit the RDMs from neural data time by time. So, can we do cross-temporal decoding based on RSA?

CTRSA-based decoding is a new algorithm for cross-temporal E/MEG decoding by RSA. We use the neural data from two different time-points to establish a Cross-Temporal Representatonal Dissimilarity Matrix (RDM) corrsponding to time i and time j. By this train of thought, we can obtain Number_of_Times by Number_of_Times Cross-Temporal RDMs. Then we can establish a Coding Model RDM by the experimental hypothesis. Finally, we can calculate the similarity between this Coding Model RDM and the Number_of_Times by Number_of_Times Cross-Temporal RDMs and obtain the cross-temporal decoding results.

## Notes
In PyCTRSA, you can not only calculate the cross-temporal similarities based on this novel methods to realize decoding, but also calculate the cross-temporal similarities based on neural data under two different conditions to see the similar data patterns between two conditions and calculate the cross-temporal similarities based on normal RDMs to see the similar representational patterns between different time-points.

## Features

**1. Calculate the Cross-Temporal RDM (Novel here!)**

> calculate CTRDMs for a single channel/subject
> calculate CTRDMs for multi-channels&subejcts

**2. Calculate the similarity between two CTRDMs (Novel here!)**

> by Pearson Correlation/Spearman Correlation/Kendall tau Correlation/Cosine Similarity/Euclidean Distance

**3. Calculate the Cross-Temporal Similarities**

> calculate CTSimilarities between neural data under two conditions
> calculate CTSimilarities based on normal RDMs
> calculate CTSimilarities between CTRDMs and a Coding Model RDM (Novel here!)

**4. Plot the Results**

> plot the CTRDM
> plot the CTSimilarities
> plot the time-by-time similarities

## How to use PyCTRSA

|   | Run the Tutorial&Demo | View the Tutorial&Demo |
| - | --- | ---- |
| Learn here! | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ZitongLu1996/PyCTRSA/blob/master/docs/Tutorial_for_PyCTRSA_colab.ipynb) | [![View the notebook](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/ZitongLu1996/PyCTRSA/blob/master/docs/Tutorial_for_PyCTRSA.ipynb) |

## Efficiency of using PyCTRSA

Here, we use a tutorial to compare the traditional classification-based decoding and novel cross-temporal RSA-based decoding below:

|   | Run the Tutorial | View the Tutorial |
| - | --- | ---- |
| Learn here! | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ZitongLu1996/PyCTRSA/blob/master/docs/Decoding_Classification_VS_CTRSA.ipynb) | [![View the notebook](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/ZitongLu1996/PyCTRSA/blob/master/docs/Decoding_Classification_VS_CTRSA.ipynb) |

## About PyCTRSA

This work should be affilliated with **[NeuroRA](https:/zitonglu1996.github.io/NeuroRA/)**, but it is an independent part.

If you have any question, find some bugs or have some useful suggestions while using, you can email me and I will be happy and thankful to know.

>My email address: 
>zitonglu1996@gmail.com / zitonglu@outlook.com

>My personal homepage:
>https://zitonglu1996.github.io
