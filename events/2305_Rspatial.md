# Why use CSC services?

* CSC specialist support
* “Outsource” heavy/specialized computations
* **Free of charge** for open science Finnish universities and research institutes

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

# Why use CSC supercomputer?

When own computer is not enough:
<br><br>

* Resource needs (time (> 2 hours), memory (> 8 GB), storage (> 50GB), GPU)
* Prebuilt environments
* Run many experiments at same time
* Data availability
* Collaboration possibility

# Allas

* Object storage 
* Up to 200TB for free
* Connected to CSC services and own computer
* Project lifetime data storage
* Data gateway to CSC environment
* Within CSC project data sharing
* Some tools support direct read from Allas
* NOT a file system, data management environment, backup service!

# Get access

Working at Finnish University / Univeristy of applied Sciences / state research institute? -> Free of charge
<br><br>

1. Create personal user account
2. Find a senior researcher / PI to create (a personal account for themselves and) and CSC project
3. Ask above person to add you to the project and add needed services
4. Read the documentation about the service in question: https://docs.csc.fi

# MyCSC

* Manage your account
* Manage your projects/services
* Estimate billing units
* Change password
* ...

[`https://my.csc.fi`](https://my.csc.fi)

# Challenges

<p align="center">

"`You can’t learn everything you need all at once.
Instead, continually learn and know when to ask for help.`"
<br> - Aalto Scientific Computing

</p>

* Linux and commandline
* get to know new system and concepts
* possibly new software/ways of working
* queuing system
* data transfer bottleneck
* ...

# Training

* ['CSC computing environment' self-study course](https://ssl.eventilla.com/csccompenvselflearn)
* ['Research data management' self-study course](https://ssl.eventilla.com/event/v8B6B)
* [CodeRefinery workshop September 2023](https://coderefinery.org/lessons/core/)
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

# Supercomputer

Main differences to own computer:
<br><br>

* Not faster, but bigger
* For speed up: parallelism
* Memory and CPU(/GPU) availability (application needs to make use of this!)
* Non-interactive for heavy computations
* Resource knowledge

# Possibilities

* Use more memory/CPU/GPU than your own computer has available <br>
<br>
-> analyse large files, Machine learning model training
<br>
* Speed up so called *embarrassingly parallel* analyses (many identical, but separate tasks) <br><br>
-> doing same thing to multiple map tiles/ data chunks

# Puhti basics

<p align="center">
  <img src="images/puhti_overview.png" width="50%">
</p>

# Applications

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

 Something missing?
      Ask us :)
      servicedesk@csc.fi
</div>

# r-env

* includes > 1100 R packages, including many geospatial packages
* [Geospatial packages documentation](https://docs.csc.fi/apps/r-env-for-gis/)
* [General r-env documentation](https://docs.csc.fi/apps/r-env/)
* [Running R scripts on Puhti- self learning examples](https://github.com/csc-training/geocomputing/tree/master/R)

-> [Instructions on additional R package installation in CSC docs](https://docs.csc.fi/apps/r-env/#r-package-installations)

# "My R code runs slow, what can be done?"

* Try to understand which part of the code takes time and why
    * Use `system.time()` or `tictoc` package
* Different R packages may provide same functions but are implemented differently (i.e. run faster/slower)
    * e.g. prefer `sf` over `sp` and `terra` over `raster`. 
* Always be suspicious of for-loops!
* Going parallel may help
* Unfortunately, increasing the number of cores will never decrease the time needed in the same proportion

# Parallelization 

Within R:
* use package future
* or snow, foreach, Rmpi,...

Outside R:
* gnuparallel
* other workflow tools can also be use, see [CSC High Throughput Computing documentation](https://docs.csc.fi/computing/running/throughput/)

# Getting started

Check out our [Geocomputing page](https://research.csc.fi/geocomputing)

* [Step by step instructions](https://research.csc.fi/en/accounts-and-projects)
* [Find your account and project information](my.csc.fi)

* [Read the docs](https://docs.csc.fi)

* check our [tutorials](https://docs.csc.fi/support/tutorials/) and [geocomputing examples](https://github.com/csc-training/geocomputing)

# Running your own R script in Puhti

(0. Get CSC user account)
1. Log in to Puhti web interface (www.puhti.csc.fi).
2. Move your data and scripts to Puhti.
3. Open RStudio.
4. Check R package availability (https://docs.csc.fi/apps/r-env-for-gis/)
	* If needed, install it yourself or ask CSC - servicedesk@csc.fi
5. Fix paths of your input/output files.
6. Test your script with some test data.
7. Write a batch job script.
8. Run your scripts with all data as batch job (or interactively)
(9. Make use of several cores using future package in your R code.)
