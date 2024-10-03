---
title: Data for Economics Projects
#subtitle: Hopefully everything you need and lots of things you hopefully won't
# https://bookdown.org/yihui/rmarkdown/html-document.html#floating-toc
layout: single
toc: true
toc_label: "Contents"
toc_min_header: 1
toc_max_header: 2
toc_sticky: true
author_profile: true
date: "2024-10-02"
---

Here's where I keep a running list of good data resources. 

Most of these data sources tend towards environmental or development economics, since that's what I'm familiar with.

I'll add to this page as new data are brought to my attention, but if you have suggestions please [email me](mailto:j.stallman@yale.edu). 


# General Data-Finding

- [Our World in Data (OWID)](https://ourworldindata.org/): OWID may well be your first stop for just about any topic. 

  - They have a wealth of subjects and data sources. If you're using data you first accessed through OWID, you'll want to cite OWID as a source, but ultimately pull your data from the source that *they* pull from to make sure you've got the latest.

- Try to find the most recent well-published paper in your area, and see what data sources they use. Recent papers will often link to a Zenodo repository with their data.

# Country-Specific Data

## Rich Countries
- [Statistics Canada](https://www150.statcan.gc.ca/n1/en/type/data): contains a wealth of data all about Canada

## Developing Countries

- [Duncan Thomas at Duke](https://ipl.econ.duke.edu/dthomas/dev_data/) has a great compilation of data from developing countries

# Agriculture

- [The US Department of Agriculture](https://www.usda.gov/): There's a reason so much research is done on the United States! The data is great! If the thing you're looking at is traded in a market in the United States, chances are pretty good the USDA is capturing something about it.
- [International Food Policy Research Institute (IFPRI)](https://dataverse.harvard.edu/dataverse/IFPRI): IFPRI has a wide range of datasets.


# Animals

## Birds
[eBird](https://science.ebird.org/en/use-ebird-data/download-ebird-data-products): Cornell and the Audobon Society's registry of over 600 million birding observations since 2002. You need to request access (which can take around a week). Once you've done that, you can use [auk](https://cornelllabofornithology.github.io/auk/), the R package for eBird analysis.

## Fish and Other Aquatics

[fishR](https://fishr-core-team.github.io/fishR/): this website has tons of great resources and data


# Atmospheric Data 

Atmospheric data is often generated as rasters (think pixels on a map). It requires an additional level of cleaning to translate these rasters into vectors (polygons like countries or points like cities) that we can run analysis on. 

`ekonomR` vignettes will contain examples of this workflow (in progress).

- [Climate Data from Copernicus (ECMWF)](https://cds-beta.climate.copernicus.eu/)
-

## Geoengineering Simulations

- [Geoengineering Large Ensemble Project (GLENS)](https://www.cesm.ucar.edu/community-projects/glens)
- [Simulations from Cornell's Engineering Lab](https://climate-engineering.mae.cornell.edu/data/)


# Energy 

- [The International Energy Agency (IEA)](https://www.iea.org/): includes carbon capture projects, critical minerals, coal, electricity, greenhouse gas emissions, energy prices, and more. Requires you to log in to access the free datasets, and then there's a tier behind a paywall. (Vignette: to add, using your own login to download a dataset behind a paywall in R)

## Greenhouse Gas Emissions

- The [Global Carbon Budget](https://globalcarbonbudget.org/) provides estimates of territorial carbon emissions, emissions from consumption, and emissions transfers. You can access the cleaned data through my R package [ekonomR](https://stallman-j.github.io/ekonomR/), and several vignettes cover its exploration.
- The [IEA](https://www.iea.org/) also has emissions estimates

## Energy Prices and Production

**United States**

- [US Energy Information Administration (EIA)](https://www.eia.gov/): contains oil and natural gas prices along with lots of information on energy production
- [National Renewable Energy Laboratory](https://www.nrel.gov/analysis/data-tools.html): has a wealth of data relating to renewable energy

- [Texas Parks and Wildlife](https://tpwd.texas.gov/gis/): tons of geocoded environmental data, all about Texas! They also have a great set of links to supplementary data that would be useful in a Texas-related analysis.

**Canada**

- [Statistics Canada: Oil Prices](https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=1810000101)

# Household Panel Surveys

Panel surveys are great because they allow us to track changes over time. They're difficult and costly to run, however, so there aren't very many high-quality ones.

- [Ghana Socioeconomic Panel Survey](https://egc.yale.edu/data/isser-northwestern-yale-long-term-ghana-socioeconomic-panel-survey-gsps): currently on the fourth wave, starts in 2009 and the most recent in 2022
- [Indonesian Family Life Survey](https://www.rand.org/well-being/social-and-behavioral-policy/data/FLS/IFLS.html): longitudinal survey of India, with waves starting in 1993
- [Mexican Family Life Survey](https://www.ennvih-mxfls.org/english/): three rounds, 2002, 2005-2006, and 2009-2012

# Opinion Surveys

- The Yale Program on Climate Communication has been running [Climate Opinion Surveys](https://climatecommunication.yale.edu/visualizations-data/ycom-us/) since 2010.



# Pollution

## Air Pollution

[AirNow.gov](https://www.epa.gov/outdoor-air-quality-data): the best first stop for air quality monitoring

[PurpleAir](https://map.purpleair.com): a map of low-cost air quality sensors that have a high correlation with industrial-quality sensors according to California's [South Coast Air Quality Management District](https://www.aqmd.gov/aq-spec/evaluations/criteria-pollutants/summary-pm). These sensors update every 2 minutes; but the downside is that the data would be a bugger to clean

To add: the latest stratospheric rasters estimates.

## Water / Other Pollution


# Trade

- [UN Comtrade](https://comtradeplus.un.org/): this is the authoritative source for trade data, but it's a bit messy to work with. 

  - If you're working with R, the R package [comtradr](https://docs.ropensci.org/comtradr/index.html) has plenty of vignettes to access the API and help you along.



# Water

**United States**

- [USGS Water Data](https://waterdata.usgs.gov/nwis): includes water quality data, water flow, levels of water and more. [Here](https://waterservices.usgs.gov/docs/) is the documentation for downloading help.

**Africa**

- [African Database of Hydrometric Indices (ADHI): 1950-2018](https://essd.copernicus.org/articles/13/1547/2021/)

# Weather

## United States

- [Spatial Hazards Events and Losses Database (SHELDUS)](https://cemhs.asu.edu/sheldus/metadata): January 1960 to Dec 2022, includes hazards like thunderstorms and tornados at the county level


