---
lang:   en
theme: csc-2019

---

# Mini-intro to possibilities of using R in CSC's supercomputer Puhti {.title}

Samantha Wittke, CSC (Geoinformatics specialist)
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0;" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>


# CSC - IT center for science

<div class="column">

* Non-profit company producing IT services for research and higher education
* Owned by ministry of education and culture (70%) and higher education institutions (30%)
* Headquaters in Keilaniemi, Espoo
* Side offices and supercomputers in Kajaani

</div>

<div class="column">

<p align="center">
  <img src="/home/samwitt/git/CSC_GIS_presentations/images/kajaani.png" width=95%">

</p>

</div>

# CSC services

[`research.csc.fi/en/service-catalog`](https://research.csc.fi/en/service-catalog)
<br></br>
<div class="column">
**Compute & Analyze**

  - cPouta / ePouta / Rahti -> Cloud 
  - Puhti / Mahti / LUMI -> Supercomputers
  - CSC Notebooks
  - Sensitive Data (SD) services
</div>
<div class="column">
**Store, Share & Publish Data**

  * Allas -> Object storage
  * Fairdata
  * Paituli
</div>

# Why use CSC services?

* CSC specialist support
* “Outsource” heavy/specialized computations
* **Free of charge** for open science Finnish universities and research institutes

# Supercomputer

Main differences to own computer:
<br><br>

* Not faster, but bigger
* For speed up: parallelism
* Memory and CPU(/GPU) availability (application needs to make use of this!)
* Non-interactive for heavy computations
* Resource knowledge

# Possibilities - supercomputer

* Use more memory/CPU/GPU than your own computer has available <br>
<br>
-> analyse large files, Machine learning model training
<br>
* Speed up so called *embarrassingly parallel* analyses (many identical, but separate tasks) <br><br>
-> doing same thing to multiple map tiles/ data chunks

# Puhti supercomputer - Basics

<p align="center">
  <img src="/home/samwitt/git/CSC_GIS_presentations/images/puhti_overview.png" width="50%">
</p>

# Puhti supercomputer - Applications

<div class="column">
* CloudCompare
* FORCE 
* GDAL/OGR
* GRASS GIS
* LasTools
* MatLab 
* OpenDroneMap
* Orfeo Toolbox
* PCL
* PDAL
</div>

<div class="column">
* Python geospatial packages: geoconda
* QGIS
* R geospatial packages: r-env
* SagaGIS
* SNAP, Sen2cor, sen2mosaic
* WhiteboxTools
* Zonation
* Deep learning: pytorch, tensorflow

 **Something missing?**
      Ask us :)
      servicedesk@csc.fi
</div>

# Puhti supercomputer - r-env

* includes > 1100 R packages, including many geospatial packages
* [Geospatial packages documentation](https://docs.csc.fi/apps/r-env-for-gis/)
* [General r-env documentation](https://docs.csc.fi/apps/r-env/)
* [Running R scripts on Puhti- self learning examples](https://github.com/csc-training/geocomputing/tree/master/R)

-> [Instructions on additional R package installation in CSC docs](https://docs.csc.fi/apps/r-env/#r-package-installations)


# Puhti supercomputer - Data availability

<div class="column">

* Large commonly used geospatial datasets with open license
* Removes transfer bottleneck
* Located at: `/appl/data/geo/`
* All Puhti users have read access

</div>
<div class="column">

* ~13 TB of datasets available:
  * Paituli data 
  * SYKE open datasets
  * LUKE Multi-source national forest inventory
  * Virtual rasters for NLS DEMs
  * Sentinel and Landsat mosaics

</div>

<br>

<div>
[List of spatial data in computing environment](https://docs.csc.fi/data/datasets/spatial-data-in-csc-computing-env/)
</div>


# Running your own R script in Puhti

0. Get CSC user account.
1. Log in to Puhti web interface (www.puhti.csc.fi).
2. Move your data and scripts to Puhti.
3. Open RStudio.
4. Check R package availability.
5. Fix paths of your input/output files.
6. Test your script with some test data.

...

# Make use of the power of Puhti

...

7. Write a batch job script.
8. Run your scripts with all data as batch job (or interactively)
9. Make use of several cores using future package in your R code, if needed.

# "My R code runs slow, what can be done?"

* Try to understand which part of the code takes time and why
    * Use `system.time()` or `tictoc` package
* Different R packages may provide same functions but are implemented differently (i.e. run faster/slower)
    * e.g. prefer `sf` over `sp` and `terra` over `raster`. 
* Always be suspicious of for-loops!
* Consider parallelization
* Understand that number of cores != multiplier of speedup

# Parallelization locally and on the supercomputer

**Within R:**

* use package `future`
* or `snow`, `foreach`, `Rmpi`,...

<br><br>

**Outside R:**

* `GNUparallel`
* other workflow tools can also be use, see [CSC High Throughput Computing documentation](https://docs.csc.fi/computing/running/throughput/)


# Training

* ['CSC computing environment' self-study course](https://ssl.eventilla.com/csccompenvselflearn)
* ['Research data management' self-study course](https://ssl.eventilla.com/event/v8B6B)
* [CodeRefinery workshop September 2023](https://coderefinery.org/lessons/core/)
* [STAC workshop](https://ssl.eventilla.com/stac_2023)
* Geocomputing with Puhti in Fall 2023
* [CSC geoinformatics training materials](https://research.csc.fi/gis-learning-materials)

<br><br>
-> follow our [training calendar](https://www.csc.fi/en/training#training-calendar)

# How we can help

* 'Z is not working as expected'
* 'My code gives error Y'
* 'Can A be installed to Puhti?'
* 'Any advice how to do X?'
* Training/example wishes

<br></br>
**-> servicedesk@csc.fi**
<br></br>
**-> [Weekly user support coffe break](https://ssl.eventilla.com/usersupportcoffee)**

[Speed up your request](https://docs.csc.fi/support/support-howto/)

# Summary - Why use a supercomputer?

<p style="font-size:40px;">&#8987; Resource needs (time, memory, storage, GPU)</p>
<p style="font-size:40px;">&#128126; “Outsource” heavy computations, keep own computer free</p>
<p style="font-size:40px;">&#127960; Prebuilt environments, application availability</p>
<p style="font-size:40px;">&#128202; Run many experiments at same time</p>
<p style="font-size:40px;">&#127760; Data availability</p>
<p style="font-size:40px;">&#128101; Collaboration possibility</p>
<p style="font-size:40px;">&#10067; CSC specialist support</p>
<p style="font-size:40px;">&#128184; Free of charge for open science at Finnish universities and research institutes.</p>


# Getting started

Visit our [Geocomputing page](https://research.csc.fi/geocomputing)

* [Step by step instructions](https://research.csc.fi/en/accounts-and-projects)
  1. Create personal user account
  2. Find a senior researcher / PI to create (a personal account for themselves and) and CSC project
  3. Ask above person to add you to the project and add needed services
* [Find your account and project information](my.csc.fi)
* [Read the docs](https://docs.csc.fi)
* Check our [tutorials](https://docs.csc.fi/support/tutorials/) and [geocomputing examples](https://github.com/csc-training/geocomputing)


