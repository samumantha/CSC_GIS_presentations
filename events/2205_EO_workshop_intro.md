--- 
title: Earth Observation user workshop
subtitle: hybrid
author: Eetu Jutila (SYKE) and Samantha Wittke (CSC)
date: 16.05.22
lang: en
theme: csc-2016
---

# Practicalities

* Let's discuss a lot
* Many presentations, but please ask questions
* Mentimeter: www.menti.com; 2773 8461
* Accessibility in hybrid event
* Slides: https://a3s.fi/gis-workshops/22_EO_workshop/EO_intro_slides.pdf , https://a3s.fi/gis-workshops/22_EO_workshop/EO_at_CSC_slides.pdf

# Today

* Introduction round
* EO data and processing (general)
* CSC resources for EO
* Use cases of EO research using CSC resources
* Discussion time / Ask us anything

# Introduction

* Who are you?
* What is your research about?
* voluntary networking: add your email-address for others to contact you.
-> www.menti.com; 2773 8461

# Geoportti and CSC


<p align="center">
  <img src="images/geoportti.png" width="50%">
</p>

* Finnish research infrastructure for geospatial research
* CSC is one of many project partners
* technical implementation
* computing support
* Geoportti webportal: [www.geoportti.fi](https://geoportti.fi)

# Getting started using EO 

1. What data are we talking about?
2. Which data to use?
3. Where to get the data?
4. How to get the data?
5. Processing EO data

# What is your level of experience with...

* optical EO
* RADAR/SAR

-> www.menti.com; 2773 8461

# EO tutorial draft

<p align="center">

  [https://hackmd.io/@GeospatialCSC/EO_tutorial](https://hackmd.io/@GeospatialCSC/EO_tutorial)

</p>

# EO data

<p align="center">
  <img src="images/fusion.jpg" width="50%">
</p>

> Credit: ESA Phi lab


# How to decide which data to use?

**What information is needed?**

* structural vs spectral characteristics
* details
* time series

**Budget?**

**Handling**

* experience 
* pre-processing needs

# What kind of EO data are you interested in?

* optical multispectral
* hyperspectral
* RADAR/SAR
* LiDAR
* other

-> www.menti.com; 2773 8461

# Where and how to get data?

* Mosaics, Markus Törmä (SYKE)
* Geocubes, Lassi Lehto (FGI/NLS)
* FinHub, Mwaba Hiltunen (FMI)  
* Paituli
* Other data sources
* Considerations
  
# Mosaics

Markus Törmä (SYKE)

# Geocubes

Lassi Lehto (FGI/NLS)

# FinHub

Mwaba Hiltunen (FMI) 

# Paituli

[www.paituli.csc.fi](https://paituli.csc.fi)

* ~13 TB data with webbased data preview
* spatial data download service
* some EO data products, possible reference data 
* open to anyone, unrestricted access
* includes historical versions of datasets
* not limited to Finland

# Other data sources

* [Copernicus Open Acces Hub](https://scihub.copernicus.eu/)
* [Earth Data NASA](https://search.earthdata.nasa.gov/search)
* [USGS Earth Explorer](https://earthexplorer.usgs.gov/)
* [Alaska Satellite Facility](https://search.asf.alaska.edu/#/)
* List at [Geoportti](https://www.geoportti.fi/data/find-and-get-data/)
* our [EO tutorial](https://hackmd.io/@GeospatialCSC/EO_tutorial)


# Download vs data and processing platforms

* Puhti, Google Earth Engine (GEE), Amazon Web Services (AWS), Sentinel Hub, DIAS-services, ...
* setup
* costs
* efficiency
* availability
  
# What to consider when choosing a place to get data from?

* download methods
* costs
* license

# What to consider when choosing a method to download data?

* Web interface or other Graphical User Interfaces (GUI)
  * visual checking
  * search parameters
* Application Programming Interfaces (API)
  * scripts
  * file lists
  
# Our suggestion

* Search in web interface 
* Download via script
* sentinelsat (Python)

# How to process the data?

* Graphical User Interfaces (GUI)
* Command Line Interfaces (CLI)
* own code: Python/R/Julia/Matlab/...

# Graphical User Interface - GUI 

* Good for testing and prototyping workflows and visualization of the results
* Problems with reproducability
* Possibility to create models/graphs and export them as scripts
* Free and open source options: SNAP, QGIS, OrfeoToolbox (OTB), ...

# Command Line Interface - CLI

* No need to code (but it helps)
* Manuals/documentation
* Acces to super- and cloud- computing 
* Eg. GDAL, FORCE, SNAP GPT, OrfeoToolbox (OTB), ...
  
# Python/R/Julia/Matlab,...

* Flexibilty 
* Reproductibility
* Parallellization
* Learning curve
* Good community support and tutorials
* Many different options and packages for EO
* Access to super- and cloud- computing 


# A few common EO processing steps

## Optical multispectral

* atmospheric correction
    -> Sen2cor, FORCE, OTB, ...
* cloud identification and masking
    -> FORCE, SNAP, Python (s2cloudless), R (sen2r), ...
* calculation of (vegetation) indices
    -> raster calculator / band math / map algebra: QGIS, SNAP, Python (rasterio, numpy), R (sen2r), ... 
* zonal statistics 
    -> QGIS, Python (rasterstats), ...

# A few common EO processing steps

## RADAR

* Radiometric Calibration
* Terrain Correction
* Inferometry
* Polarimetry

-> SNAP, sarpy, OTB etc.

# A few common EO processing steps

## Any

* download
    -> Python (sentinelsat), R (sen2r), ...
* mosaicing
    -> Python (sen2mosaic, sen1mosaic), ...

# What software do you use and for what?

-> www.menti.com; 2773 8461
