# Using dipy to explore Diffusion Weighted Imaging and Tractography

Matteo Visconti di Oleggio Castello & Manon de Villemejane

------
This repository contains a jupyter notebook with a quick tutorial on how to use [`dipy`](http://www.nipy.org/dipy) to perform tractography on diffusion weighted imaging.

We presented this tutorial during the 2017 Psychological & Brain Science "Day of Graduate Research Roundtable" at Dartmouth College. It's very much an exploration, and care should be taken before using any of these methods in real research—know thy methods. However, I believe we learned a lot about the methods by messing around. We hope it will be helpful for you as well.



## Required packages

You should need only `dipy` to run the analyses, and [`datalad`](http://www.datalad.org) to download the data. Some steps might require a working copy of FSL or your favourite neuroimaging toolbox to perform skull stripping and tissue segmentation.

We provide a conda [`environment.yml`](environment.yml) file that allows you to re-create the conda environment we used to run this tutorial. You should be able to create it using
```
conda env create -f environment.yml
```
It will be big because it's based on anaconda, so it will install a lot of packages that this tutorial doesn't use. For more information on how to manage conda environment, check this page: https://conda.io/docs/using/envs.html
