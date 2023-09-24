---
lang:   en
theme: csc-2019
---

# Overview of CSC geocomputing resources {.title}

Samantha Wittke, CSC (Geoinformatics specialist),<br> Geospatial challengecamp kickoff 26.09.23 <br>
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0;" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>

# Outline

1. CSC service overview
2. Supercomputers
3. Data
4. Training and support
5. Mentoring

# CSC services

[`research.csc.fi/en/service-catalog`](https://research.csc.fi/en/service-catalog)

<br></br>
<div class="column">
**Compute & Analyze**

* <p style="font-size:40px;"> Webservices, virtual machines in the cloud: `cPouta / ePouta / Rahti` </p>
* <p style="font-size:40px;"> Heavy computations on the supercomputer: `Puhti / Mahti / LUMI` </p>
* <p style="font-size:40px;"> Teaching and collaborating: `CSC Notebooks` </p>
</div>
<div class="column">
**Store, Share & Publish Data**

* <p style="font-size:40px;"> Project lifetime data storage: `Allas` </p>
* <p style="font-size:40px;"> Share and publish data: `Fairdata`</p>
* <p style="font-size:40px;"> Share and publish geospatial data: `Paituli`</p>
</div>

<br>

<div><p style="font-size:40px;">Working with privacy related data: `Sensitive Data (SD) services`</p></div>

# Why use CSC services?

* CSC specialist support
* “Outsource” heavy/specialized computations
* **Free of charge** for open science Finnish universities and research institutes


# Why use a supercomputer?

<p style="font-size:40px;">&#8987; Resource needs (time, memory, storage, GPU)</p>
<p style="font-size:40px;">&#128126; “Outsource” heavy computations, keep own computer free</p>
<p style="font-size:40px;">&#127960; Prebuilt environments, application availability</p>
<p style="font-size:40px;">&#128202; Run many experiments at same time</p>
<p style="font-size:40px;">&#127760; Data availability</p>
<p style="font-size:40px;">&#128101; Collaboration possibility</p>
<p style="font-size:40px;">&#10067; CSC specialist support</p>
<p style="font-size:40px;">&#128184; Free of charge for open science at Finnish universities and research institutes.</p>



# Supercomputers

<br><br><br>

<p align="center">
<b>Puhti - Mahti - LUMI</b>
</p>

# Puhti

<div class="column">

<p align="center">
  <img src="../images/puhti_a4.jpg" width="55%">
</p>

</div>

<div class="column" >

<br>

* Use cases from interactive single core data processing to medium scale parallel simulations
* `~28 000` Intel CPUs 
* `240` Nvidia V100 GPUs 
* wide stack of pre-installed software
</div>

# Puhti webinterface 

<p>&rarr; check your data, testing, code development, file management, quotas, apps</p>

<p align="center">
[`https://puhti.csc.fi`](https://puhti.csc.fi)
</p>

<p align="center">
  <img src="../images/puhti_webinterface_overview.png" width="55%">
</p>


# Puhti applications

<div class="column">
* CloudCompare
* FORCE 
* GDAL/OGR
* GRASS GIS
* Julia
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

<p><b>Something missing? &rarr; Ask us :) </b></p>

</div>

# Data available on Puhti

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
  * NLS Virtual rasters for DEMs
  * Sentinel and Landsat mosaics

</div>

<br>

<div>
[List of spatial data in computing environment](https://docs.csc.fi/data/datasets/spatial-data-in-csc-computing-env/)
</div>

# Mahti

<div class="column">

<p align="center">
  <img src="../images/mahti_a4.jpg" width="55%">
</p>

</div>

<div class="column">

<br>

* Geared towards medium and large scale parallel simulations
* `~90 000` Intel CPUs
* `96` Nvidia A100 GPUs 
* some pre-installed software

</div>

# LUMI

<div class="column">

<p align="center">
  <img src="../images/lumi2.jpg" width="95%">
</p>
</div>

<div class="column">

<br>

* Research + industry and SME access
* `~100 000`  AMD EPYK CPUs
* `~10 000` AMD MI250X GPUs
* Some pre-installed software
</div>

# Skills

<p align="center">

"`You can’t learn everything you need all at once.
Instead, continually learn and know when to ask for help.`"
<br> - Aalto Scientific Computing

</p>
<br>

* <p style="font-size:40px;">Linux and commandline</p>
* <p style="font-size:40px;">Get to know new system and concepts</p>
* <p style="font-size:40px;">Possibly new software / ways of working</p>
* <p style="font-size:40px;">Data transfer </p>
* <p style="font-size:40px;">...</p>

# Harnessing the power

<div class="column">

Supercomputer != laptop


<br><br>

&rarr; [Geocomputing course 12.+13. October 2023](https://challenge-camp.geoportti.fi/en/latest/tabs/schedule.html#data-science-training-at-csc)
</div>

<div class="column">



<p align="center">
  <img src="../images/cc_reg.png" width="95%">
</p>
</div>

# Data - Acquisition

<div class="column">

Non-CSC services: 
<br>

* `paikkatietohakemisto.fi`
* `avoindata.fi`
* Statistics Finland paikkatietoainesto

</div>
<div class="column">



<p align="center">
  <img src="../images/pth.png" width="95%">
</p>
</div>

# Data - Acquisition


<div class="column">
<br>

FAIRDATA services<br><br>
&rarr; Paituli spatial data download service<br>
`paituli.csc.fi`

</div>
<div class="column">

<p align="center">
  <img src="../images/paituli.png" width="75%">
</p>

</div>

# Data - Storage

<div class="column">


* On disk for frequent use <br>

* Object storage Allas
  * Data gateway to CSC environment
  * Up to 200TB for free
  * Project lifetime storage
  * Some tools support direct read from Allas
  * NOT a file system, data management environment, backup service

</div>

<div class="column">

<p align="center">
  <img src="../images/CSC_service_icon_allas.png" width="95%">
</p>
</div>


# Training

* ['CSC computing environment' self-study course](https://ssl.eventilla.com/csccompenvselflearn)
* ['Research data management' self-study course](https://ssl.eventilla.com/event/v8B6B)
* [CodeRefinery materials for FAIR research software development practices](https://coderefinery.org/lessons/core/)
* [CSC geoinformatics training materials](https://research.csc.fi/gis-learning-materials)

<br><br>
&rarr; follow our [training calendar](https://www.csc.fi/en/training#training-calendar)

# Support


[`docs.csc.fi`](https://docs.csc.fi)

[`research.csc.fi`](https://research.csc.fi)

[`github.com/csc-training/geocomputing`](https://github.com/csc-training/geocomputing)

<br>

\+ servicedesk@csc.fi

\+ User support session in Zoom every Wednesday at 14.00

# Mentoring

<div class="column">

<br>

Email to: <br><br>

servicedesk@csc.fi<br>
CC: giscoord@csc.fi


</div>

<div class="column">

<br>

We are happy to offer mentoring sessions: <br><br>

* Technical level
* Service and tools choice
</div>

# Thank you for your attention! 
<div class="column">

<br>

<p>Questions? &rarr; ask now or contact `servicedesk@csc.fi` </p>

<br>

<p align="center">
  <img src="../images/csc.png">
</p>

</div>

<div class="column">


<p align="center">
  <img src="../images/geoportti.png">
</p>
<p align="center">
  <img src="../images/lih.png">
</p>
</div>