---
lang: en
theme: csc-2016
title: Earth Observation @ CSC
subtitle: Storage and computing services
date: 16.05.2022
author: Samantha Wittke (CSC)
---


# CSC 

* non-profit state enterprise with special tasks
* owned by Finnish state (70%) and higher education institutions (30%)
* headquaters in Keilaniemi, Espoo
* side offices and supercomputers in Kajaani

# CSC services

[`research.csc.fi/en/service-catalog`](https://research.csc.fi/en/service-catalog)

<div class="column">
**Compute & Analyze**

  - cPouta / ePouta
  - Puhti / Mahti / LUMI
  - CSC Notebooks
  - Rahti

</div>

<div class="column">
**Store, Share & Publish Data**

  * Allas
  * EUDAT
  * IDA
  * Paituli

</div>

\+ Sensitive Data (SD) services


# Storing EO data

Allas object storage

* during project lifetime
* CSC account and project required
* access from other services and own computer
* some tools can read directly from Allas
* data is immutable
* Maximum size for free: **200TB**

[Allas and Geospatial data webinar](https://www.youtube.com/watch?v=mnFXe2-dJ_g)


# Key to efficient geocomputing

<p align="center">
  <img src="images/gui_to_script.png" width="65%">
</p>


# EO data processing and analysis

<p align="center">
  <img src="images/puhti_pouta_table.png" width="65%">
</p>


# Pouta cloud

<div class="column">

* Virtual Machines
* available on demand
* under own administration
* ideal for webserver / databases

</div>

<div class="column">
<p align="center">
  <img src="images/cloud.png" width="65%">
</p>

</div>

# Why use Puhti?

When own computer is not enough:

* Resource needs (time (> 2 hours), memory (> 8 GB), storage (> 50GB))
* prebuilt environments
* parallelization
* data availability (Paituli)

**-> Outsource heavy computations, keep own computer free**

It’s **free**! (for open science at Finnish higher education and state research institutes)

# Puhti supercomputer

**Main differences to laptop:**

* memory and CPU(/GPU) availability (software needs to make use of this!)
* non-interactive
* resource knowledge

# Computing solutions - Puhti


<p align="center">
  <img src="images/puhti_overview.png" width="50%">
</p>

# Puhti webinterface 

-> check your data, testing, code development, file management, quotas, apps

[`puhti.csc.fi`](https://puhti.csc.fi)

<p align="center">
  <img src="images/puhti_webinterface.png" width="50%">
</p>

# Software

[List of Applications in Docs](https://docs.csc.fi/apps/#geosciences)

<div class="column">
* **FORCE & SPLITS**
* **GDAL / OGR**
* LasTools 
* MatLab / Octave
* Mapnik
* OpenDroneMap
* **OrfeoToolbox**
* PCL
</div>
<div class="column">
* PDAL
* CloudCompare
* **QGIS**
* SagaGIS
* **SNAP, Sen2cor**
* **WhiteboxTools**
* Zonation
* ...
</div>

# Python

<div class="column">

[Geoconda](https://docs.csc.fi/apps/geoconda/)

</div>

<div class="column">

<p align="right">
  <img src="images/python.jpg" width="20%">
</p>

</div>

* about 600 packages
* for raster, vector, pointcloud processing
* \+ scikit and other data science packages

other modules:

* Deep learning: [tensorflow](https://docs.csc.fi/apps/tensorflow/), [pytorch](https://docs.csc.fi/apps/pytorch/)
-> have geopandas, rasterio

You can also create own environment / install own software! -> [Tykky](https://docs.csc.fi/computing/containers/tykky/)

# R environment on Puhti

<div class="column">

* R and RStudio Server
* 1300+ R packages
* Pre-installed libraries / software required by R packages
* Mathematics library for faster calculations (Intel® OneMKL)
* TensorFlow (for using [the R Interface to Tensorflow](https://tensorflow.rstudio.com/))

</div>

<div class="column">

<p align="right">
  <img src="images/R.jpg" width="40%">
</p>

</div>

# Data

almost all data from [Paituli](https://paituli.csc.fi) on Puhti +

* SYKE open datasets
* LUKE Multi-source national forest inventory
* NLS Virtual rasters for DEMs

-> '/appl/data/geo'

Sentinel-2 L2A (agricultural Finland, 2016-2021)

-> [Allas](https://a3s.fi/sentinel-readme/README.txt)

[List of Geoscience data sets available from CSC computing environment](https://docs.csc.fi/data/datasets/spatial-data-in-csc-computing-env/)


# What data would you be interested to have available on Puhti/Allas?

-> www.menti.com; 2773 8461

# Common EO challenges

* many tiles, same process
-> "embarassingly parallel" -> Array jobs
* huge "dataframes"
-> dask(Python)/future(R)
* data transfer
-> Allas

# Get access

[Step by step instructions ](https://research.csc.fi/en/accounts-and-projects)

* Account 
* Project
* Resources
* Services
* [Find your account and project information](my.csc.fi)
* [Read the docs](https://docs.csc.fi)
* check our [tutorials](https://docs.csc.fi/support/tutorials/) and [geocomputing examples](https://github.com/csc-training/geocomputing)

# CSC expertise

...at your fingertips:

<div class="column">
[`docs.csc.fi`](https://docs.csc.fi)

[`research.csc.fi`](https://research.csc.fi)

</div>

<div class="column">
**\+ servicedesk@csc.fi**

* Geoinformatics team
* Data analytics and AI team
* Storage team
* Supercomputer team
* Cloudcomputing team
* Accounts team
* ...

</div>

# How we can help

<div class="column">
* 'Z is not working as expected'
* 'my code gives error Y '
* 'can A be installed to Puhti?'
* 'any advice how to do X?'
* training/example wishes

**-> servicedesk@csc.fi**
</div>

<div class="column">


* Setting up pipelines, product provision, R&D, ...

**-> CSC as project partner / subcontractor**
</div>

<p>

[Speed up your request](https://docs.csc.fi/support/support-howto/)

</p>

# How you can help


If you used any of our resources for your research, please acknowledge CSC and Geoportti in your publications, it is important for project continuation and funding reports. As an example, you can write:

<p align="center">

"The authors wish to thank CSC - IT Center for Science, Finland (urn:nbn:fi:research-infras-2016072531) and the Open Geospatial Information Infrastructure for Research (Geoportti, urn:nbn:fi:research-infras-2016072513) for computational resources and support".

</p>

# Training

* ['Using CSC environment efficiently' course](https://csc-training.github.io/csc-env-eff/)
* [18.05: Webinar - CSC´s generic services for storing, sharing and publishing data](https://ssl.eventilla.com/event/pEAl3)
* [09.-10.06: Fundamentals of Machine Learning](https://ssl.eventilla.com/mlfundamentals)
* [CSC geoinformatics training material](https://research.csc.fi/gis-learning-materials)

-> follow our [training calendar](https://www.csc.fi/en/training#training-calendar)

# Summary


<div class="column">
Puhti is an excellent tool if you

* need more computing power
* don’t want to run long analyses on your personal computer
* have a lot of data
* are using data provided on Puhti/Allas in large quantities
* are willing to use scripts and have some basic Linux skills
* are willing to learn to use Puhti
</div>
<div class="column">
Pouta is an excellent tool if you

* want to use databases and web-/mapservices
* have linux server administration skills
</div>


# Earth Observation Data Information extractor

<div class="column">

[Preprint](http://dx.doi.org/10.2139/ssrn.4067133), 
[Gitlab](https://gitlab.com/fgi_nls/public/EODIE), 
[Docs](https://eodie.readthedocs.io/)

EODIE is a toolkit to extract object based timeseries information from Earth Observation data.

* objects as polygons 
* timeframe of interest 
* features (eg vegetation indices) 
 -> per polygon timeseries of the selected features over the timeframe of interest

</div>

<div class="column">

![](images/EODIE_example.png)

</div>
