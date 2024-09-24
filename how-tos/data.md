---
title: Data Sources
#subtitle: Hopefully everything you need and lots of things you hopefully won't
# https://bookdown.org/yihui/rmarkdown/html-document.html#floating-toc
layout: single
toc: true
toc_label: "Contents"
toc_sticky: true
author_profile: true
date: "2024-09-23"
---

# Good Data Sources for (Environmental) Projects

Here's where I'll keep a running list of good data resources. I'll continue adding to this page, but if you have suggestions please [email me](mailto:j.stallman@yale.edu).

## General Data

[Our World in Data (OWID)](https://ourworldindata.org/): OWID may well be your first stop for just about any topic. 

They have a wealth of subjects and data sources. If you're using data you first accessed through OWID, you'll want to cite OWID as a source, but ultimately pull your data from the source that *they* pull from to make sure you've got the latest.

A good place to start is to find the most recent well-published paper in your area, and check out what data sources they use. Recent papers will often link to a Zenodo repository with their data.

## Trade Data

[UN Comtrade](https://comtradeplus.un.org/): all the trade data you could possibly want. 

On my list of things to do: put a UN Comtrade cleaning sequence into an `ekonomR` vignette. Email if you've got one handy!


## Carbon Tax / Emissions Trading Data

## Climate Data

Climate data is often generated as rasters (think pixels on a map). It requires an additional level of cleaning to translate these rasters into vectors (polygons like countries or points like cities) that we can run analysis on. 

`ekonomR` vignettes will contain examples of this workflow (in progress).

[Climate Data from Copernicus (ECMWF)](https://cds-beta.climate.copernicus.eu/)

## Geoengineering Simulations

[Geoengineering Large Ensemble Project (GLENS)](https://www.cesm.ucar.edu/community-projects/glens)
[Simulations from Cornell's Engineering Lab](https://climate-engineering.mae.cornell.edu/data/)


## Energy Price Data

[US Energy Information Administration (EIA)](https://www.eia.gov/): contains oil and natural gas prices along with lots of information on energy production

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