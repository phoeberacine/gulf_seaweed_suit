# gulf_seaweed_suit

Seaweed suitability map of the Gulf of Mexico.

### Usage

<code>data_processing.Rmd</code> Takes in raw polygon and raster files and reprojects, crops, and masks them to the Gulf of Mexico EEZ. Polygons are rasterized to binary rasters where 1 is where the polygon was and 0 is empty cells.

<code>scraping.Rmd</code> Sea Surface Temperature (SST) and salinity data is from [HYCOM](https://www.hycom.org/data/gomu0pt04/expt-50pt1). 

<code>Suitability_hycom.Rmd</code> SST and salinity data from HYCOM and all other rasters resampled to be same resolution. Reclassifies oceanographic rasters to be binary depending on specific seaweed thresholds set at the top of the Rmd. Creates suitability, human acitvies areas "exclusion areas", and both suitability and exclusion maps.

#### Note about Data

All data is from publically available sources.

*Oceanographic*

SST & Salinity, HYCOM: https://www.hycom.org/data/gomu0pt04/expt-50pt1

*Human Activities ("Exclusion Areas")*

EEZ, NOAA: https://inport.nmfs.noaa.gov/inport/item/54383

EEZ, Marine Regios: http://www.marineregions.org/downloads.php

Gulf of Mexico Area, Marine Regios: http://www.marineregions.org/gazetteer.php?p=details&id=4288

Artifical reefs, NOAA: https://coast.noaa.gov/digitalcoast/data/artificialreefs.html

Marine Protected Area, NOAA: https://marineprotectedareas.noaa.gov/media/data/MPAI2017.zip

Shipping Fairways, NOAA: https://inport.nmfs.noaa.gov/inport/item/39986

Oil and Gas Platforms, NOAA/BOEM: https://inport.nmfs.noaa.gov/inport/item/54390

Oil and Gas Wells, NOAA/BOEM: https://inport.nmfs.noaa.gov/inport/item/54392

Submarine Cables, NOAA: https://inport.nmfs.noaa.gov/inport/item/57238

Cable areas, NOAA: https://inport.nmfs.noaa.gov/inport/item/54402

Pipeline areas, NOAA: https://inport.nmfs.noaa.gov/inport/item/54395

Danger and Restricted Zones, NOAA: https://inport.nmfs.noaa.gov/inport/item/48876

