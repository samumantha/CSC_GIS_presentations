# Welcome 

* This workshop is on-site (SYKE,LUKE) + online 
* Schedule <br>
-> [`https://ssl.eventilla.com/event/pEb7a](https://ssl.eventilla.com/event/pEb7a)
* Q&A: HedgeDoc <br>
-> [`https://siili.rahtiapp.fi/spatialCSC22`](https://siili.rahtiapp.fi/spatialCSC22)
* Reminder about hands-on session; link to survey: <br>
[`https://link.webropolsurveys.com/S/C4755A51FB4A6DFC`](https://link.webropolsurveys.com/S/C4755A51FB4A6DFC)
* Greetings from the organizers

# Code of conduct

We strive to follow the [Code of Conduct developed by The Carpentries organisation](https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html) to foster a welcoming environment for everyone. In short: <br><br>

- Use welcoming and inclusive language
- Be respectful of different viewpoints and experiences
- Gracefully accept constructive criticism
- Focus on what is best for the community
- Show courtesy and respect towards other community members

# Goals

In the end you hopefully know more about...
<br><br>

* What kind of services are offered by CSC and Geoportti
* How these services might benefit your work
* The supercomputer and how to start using it
* What spatial data and data services are available


# CSC Account

[`https://link.webropolsurveys.com/S/C4755A51FB4A6DFC`](https://link.webropolsurveys.com/S/C4755A51FB4A6DFC)

# CSC services introduction for new users

* What services are available and what are they used for?
* How can I get access?
* What skills do I need to use the supercomputer?
* Puhti supercomputer basics

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

# Skills needed

<p align="center">

"`You can’t learn everything you need all at once.
Instead, continually learn and know when to ask for help.`"
<br> - Aalto Scientific Computing

</p>

* Using CSC computing resources: general Linux commands
* Supercomputer
    * serial & 'embarassingly parallel' tasks: general Linux commands, basic HPCterminology
    * parallel work: High Performance Computing (HPC), scientific coding
* Virtual Machines (VM): Linux administration

# Training

* ['CSC computing environment' self-study course](https://ssl.eventilla.com/csccompenvselflearn)
* ['Research data management' self-study course](https://ssl.eventilla.com/event/v8B6B)
* [CodeRefinery workshop March 2023](https://coderefinery.org/lessons/core/)
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

# Modules

Applications in Puhti are provided in modules. Use

<br>

`module load <modulename>`

<br>

before every application use to make application available.

Check [`https://docs.csc.fi/apps`](https://docs.csc.fi/apps) for module names and versions.

# Puhti basics

<p align="center">
  <img src="images/puhti_overview.png" width="50%">
</p>

# Directories

<br>

* HOME – most important (small) files, personal access only
* PROJAPPL – project specific / your installations/ shared binaries
* SCRATCH – main working area, can be used to share with project members

# Jobs and queueing 

* **Batch** jobs
	* resource request
	* computing step(s)
* Queue for resource management system to grant resources
* All heavy computing must be done via batch jobs!

# Example sbatch script

<p align="center">
  <img src="images/sbatch_script.png" width="80%">
</p>

<br>
-> File `simple_serial.bash` <br>
-> Submit for computation with `sbatch simple_seria.bash`

# Puhti web interface

-> Check your data, testing, code development, file management, quotas, graphical applications

[`puhti.csc.fi`](https://puhti.csc.fi)

<p align="center">
  <img src="images/puhti_webinterface.png" width="50%">
</p>

# Take-home Message

* Manage your CSC services via our CSC customer portal at MyCSC
* Resources are free for open science research (academic use)
* Participate in CSC trainings, read materials and watch webinars 
* Take advantage of CSC docs pages
* Contact our helpdesk for support and guidance

# How you can help

<p align="center">

"`The authors wish to thank CSC - IT Center for Science, Finland (urn:nbn:fi:research-infras-2016072531) and the Open Geospatial Information Infrastructure for Research (Geoportti, urn:nbn:fi:research-infras-2016072513) for computational resources and support`".

</p>

# Feedback

Please give us feedback via the HedgeDoc! :)

