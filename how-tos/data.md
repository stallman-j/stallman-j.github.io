---
title: Data Sources
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

# Data Sources for (Environmental) Projects

Here's where I keep a running list of good data resources. I'll continue adding to this page, but if you have suggestions please [email me](mailto:j.stallman@yale.edu).

## The Usual First Stops: General Data

- [Our World in Data (OWID)](https://ourworldindata.org/): OWID may well be your first stop for just about any topic. 

  - They have a wealth of subjects and data sources. If you're using data you first accessed through OWID, you'll want to cite OWID as a source, but ultimately pull your data from the source that *they* pull from to make sure you've got the latest.

  - A good place to start is to find the most recent well-published paper in your area, and check out what data sources they use. Recent papers will often link to a Zenodo repository with their data.

## Trade

- [UN Comtrade](https://comtradeplus.un.org/): this is the authoritative source for trade data, but it's a bit messy to work with. 

  - If you're working with R, the R package [comtradr](https://docs.ropensci.org/comtradr/index.html) has plenty of vignettes to access the API and help you along.


## Climate

### Emissions
- The [Global Carbon Budget](https://globalcarbonbudget.org/) provides estimates of territorial carbon emissions, emissions from consumption, and emissions transfers. You can access the cleaned data through my R package [ekonomR](https://stallman-j.github.io/ekonomR/), and several vignettes cover its exploration.

- The International Energy Agency[IEA] (emissions) (behind )

### Opinions

- The Yale Program on Climate Communication has been running [Climate Opinion Surveys](https://climatecommunication.yale.edu/visualizations-data/ycom-us/) since 2010.


### Climate Data 

Climate data is often generated as rasters (think pixels on a map). It requires an additional level of cleaning to translate these rasters into vectors (polygons like countries or points like cities) that we can run analysis on. 

`ekonomR` vignettes will contain examples of this workflow (in progress).

- [Climate Data from Copernicus (ECMWF)](https://cds-beta.climate.copernicus.eu/)
- 

#### Geoengineering Simulations

- [Geoengineering Large Ensemble Project (GLENS)](https://www.cesm.ucar.edu/community-projects/glens)
- [Simulations from Cornell's Engineering Lab](https://climate-engineering.mae.cornell.edu/data/)


## Energy 

### Energy Prices and Production

#### United States

- [US Energy Information Administration (EIA)](https://www.eia.gov/): contains oil and natural gas prices along with lots of information on energy production
- [National Renewable Energy Laboratory](https://www.nrel.gov/analysis/data-tools.html): has a wealth of data relating to renewable energy

- [Texas Parks and Wildlife](https://tpwd.texas.gov/gis/): tons of geocoded environmental data, all about Texas! They also have a great set of links to supplementary data that would be useful in a Texas-related analysis.

## Water

### United States

- [USGS Water Data](https://waterdata.usgs.gov/nwis): includes water quality data, water flow, levels of water and more. [Here](https://waterservices.usgs.gov/docs/) is the documentation for downloading help.

### ROW

- [African Database of Hydrometric Indices (ADHI): 1950-2018](https://essd.copernicus.org/articles/13/1547/2021/)


## Agriculture

[The US Department of Agriculture](https://www.usda.gov/): There's a reason so much research is done on the United States! The data is great! If the thing you're looking at is traded in a market in the United States, chances are pretty good the USDA is capturing something about it.


## Animals

### Birds
[eBird](https://science.ebird.org/en/use-ebird-data/download-ebird-data-products): Cornell and the Audobon Society's registry of over 600 million birding observations since 2002. You need to request access (which can take around a week). Once you've done that, you can use [auk](https://cornelllabofornithology.github.io/auk/), the R package for eBird analysis.

### Fish and Other Aquatics

[fishR](https://fishr-core-team.github.io/fishR/): this website has tons of great resources and data


## Pollution

### Air Pollution

[AirNow.gov](https://www.epa.gov/outdoor-air-quality-data): the best first stop for air quality monitoring

[PurpleAir](https://map.purpleair.com): a map of low-cost air quality sensors that have a high correlation with industrial-quality sensors according to California's [South Coast Air Quality Management District](https://www.aqmd.gov/aq-spec/evaluations/criteria-pollutants/summary-pm). These sensors update every 2 minutes; but the downside is that the data would be a bugger to clean

To add: the latest stratospheric rasters estimates.

### Water / Other Pollution


# Just for fun

- If you feel fondness towards modern-day dinosaurs and appreciate quirkiness, you might enjoy [Rosemary Mosco's monthly bird newsletter](https://newsletter.rosemarymosco.com/).

- R got you down? Or are you an instructor teaching data/R and you are seeking an excuse to procrastinate with funny pictures that may make their way into your lectures? Then check out [Allison Horst's artwork](https://allisonhorst.com/everything-else)
