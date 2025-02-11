---
lang:   en
theme: csc-2019
---

# Overview of CSC computational resources for research {.title}

Samantha Wittke, CSC (Research Software Engineer),<br> Geospatial challengecamp kickoff February 2025 <br>
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0;" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>

# Outline

1. CSC services for research overview
2. Puhti- a supercomputer
3. Data
4. Training and support
5. Mentoring

# CSC services for research

**Compute & Analyze**
  
* Supercomputers for fast and large simulations, data analysis and more: 
    * [Puhti](https://research.csc.fi/-/puhti) - a good starting point, large collection of pre-installed software, national 
    * [Mahti](https://research.csc.fi/-/mahti), national
    * [LUMI](https://www.lumi-supercomputer.eu/) , owned by the European High-Performance Computing Joint Undertaking (EuroHPC JU), hosted in Finland
* Virtual machines for web services and database: [cPouta](https://research.csc.fi/-/cpouta)
* Container cloud for scalable web services : [Rahti](https://research.csc.fi/-/rahti)
* Sensitive data: [SD services](https://research.csc.fi/sensitive-data-services-for-research), [ePouta](https://research.csc.fi/-/epouta)
* Quantum learning machine: [Kvasi](https://research.csc.fi/-/kvasi)

#  CSC services for research 

**Store, Share & Publish Data**
* [CSC Data Management main page](https://research.csc.fi/data-management) and [video playlist](https://www.youtube.com/watch?v=K-kEvfaUJdA&list=PLD5XtevzF3yEZw-8LadtaGVV8Um6CbMja) 
* Project lifetime data storage: [Allas](https://research.csc.fi/-/allas)
* Databases: [Pukki](https://docs.csc.fi/cloud/dbaas/) ([Kaivos](https://research.csc.fi/-/kaivos))
* Publishing (with access management), storing or finding data according to FAIR (Findable Accessible Interoperable Reusable) principles: [OKM Fairdata](https://www.fairdata.fi/en/): 
    * IDA: Store your data 
    * Etsin: Find data
    * Qvain: Describe your data
    * PAS: Preserve your data
* Sending data: [Funet FileSender](https://filesender.funet.fi/)
* Sensitive data: [SD services](https://research.csc.fi/sensitive-data-services-for-research)
* [Research information hub](https://research.fi/en/)

# Why use CSC services?

* CSC specialist support
* Limited resources on own computer
* “Outsource” heavy/specialized computations
* Easier collaboration
* **Free of charge** for open science at Finnish universities and research institutes

# Why use a supercomputer?

<p style="font-size:40px;">&#8987; Resource needs (time, memory, storage, GPU)</p>
<p style="font-size:40px;">&#128126; “Outsource” heavier computations, keep own computer free</p>
<p style="font-size:40px;">&#127960; Prebuilt environments, application availability</p>
<p style="font-size:40px;">&#128202; Run many experiments at same time</p>
<p style="font-size:40px;">&#128101; Collaboration possibility</p>
<p style="font-size:40px;">&#10067; CSC specialist support</p>
<p style="font-size:40px;">&#128184; Free of charge for you.</p>

# Supercomputers

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

Supercomputer != laptop

<br><br>

&rarr; [CSC computing environment self-learning course](https://csc.fi/en/training-calendar/csc-computing-environment-self-learning/)


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

* ['CSC computing environment' self-study course](https://csc.fi/en/training-calendar/csc-computing-environment-self-learning/)
* ['Research data management' self-study course](https://csc.fi/en/training-calendar/cscs-self-study-research-data-management-course/)
* [CodeRefinery workshop; collaborating on research coding projects and making your code more reusable](https://coderefinery.github.io/2025-03-25-workshop/); [materials](https://coderefinery.org/lessons/core/)
* [CSC geoinformatics training materials](https://docs.csc.fi/support/training-material/#geoscience)

<br><br>
&rarr; follow our [training calendar](https://www.csc.fi/en/training#training-calendar)

# Support


[`docs.csc.fi`](https://docs.csc.fi)

[`research.csc.fi`](https://research.csc.fi)

[`github.com/csc-training/geocomputing`](https://github.com/csc-training/geocomputing)

<br>

\+ servicedesk@csc.fi

\+ [General user support sessions](https://csc.fi/en/training-calendar/csc-research-support-coffee-every-wednesday-at-1400-finnish-time-2-2/) in Zoom every Wednesday at 14.00

# Mentoring

<div class="column">

<br>

Email to: <br><br>

servicedesk@csc.fi<br>
CC: samantha.wittke@csc.fi
Subject: mention Geospatial Challenge Camp or GCC

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
