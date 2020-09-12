# Estimating average energy use by property type in England

James Thomas  
19th August 2020

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Licence CC BY-SA 4.0" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>

Datasources may have specific licenses - see the [references list](notebooks/average_energy_use_by_property_type.ipynb#References) for more information.

## Summary

Using published statistics for each of the nearly 34,000 Lower Super Output Areas (LSOAs) in England, I have estimated the annual gas and electricity use of the average domestic property by building type (detached, semi-deteched, terraced, flat, bungalow). Specifically, I created a model using council tax property type data and Index of Multiple Deprivation data for each LSOA, supplemented by 20-year average regional heating degree day (DDH) data, to predict median annual gas and electricity comsumptions of that LSOA. I then used this model to estimate average gas and electricity use for each property type.

## Repo structure
* `notebooks` - contains the [modelling](notebooks/average_energy_use_by_property_type.ipynb) notebook and supporting notebooks.
* `raw_data` - contains the raw data downloaded from various sources (see [References](notebooks/average_energy_use_by_property_type.ipynb#References)).
* `map_data` - contains a raster map of DDH regions, plus georeferencing.
* `models` - cached models.
