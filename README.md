# School Risk Index – Capstone Project Repository

This repository contains the code and main output files for the School Risk Index—a capstone project by [Madison Buchholz](mailto:madison.buchholz@nyu.edu) and [Ole Siever](mailto:ole.siever@nyu.edu), graduate students at the [NYU Center for Urban Science + Progress](https://engineering.nyu.edu/research-innovation/centers/cusp), in cooperation with the [Institute for Development Impact](https://i4di.org) (I4DI). The project calculates a composite risk index that estimates the exposure of schools around the world to climate and environmental hazards.


## Main Code Files

- `01_Calculating School Exposure.ipynb`  
  Contains the code overlaying school location data with climate hazard exposure rasters to calculate binary hazard exposure (yes/no) for each school.

- `02_Index Calculation.ipynb`  
  Contains the code aggregating school-level exposure data to the country-level and calculating the composite School Risk Index, including individual hazard scores.

***Note:** A third notebook containing the code for two case study analyses has been excluded from this public repository due to the internal nature of part of the data involved.*



## Input Data: `0001_BASE DATA FILES/`

Due to size constraints, the full input data required to run the notebooks—including all climate hazard exposure rasters—is stored externally.

The full base data library can be accessed using the following link:
[SRI Base Data Library](https://olewelo.thegood.cloud/s/Am6THox9cSmaPcG)

This includes:
- Raw data and processing outputs used to calculate school locations.
- Climate hazard base and exposure rasters for heatwaves, air pollution, flooding, cyclones, and water scarcity, along with the code to generate them.

The folder structure in this repository matches that of the external data library. To run the notebooks, simply place the downloaded files into the 0001_BASE DATA FILES/ folder.

***Note:** While all base data files themselves are stored externally, the code used to generate the school location dataset is also included directly in this repository for reference. You can find it in: 0001_BASE DATA FILES/01_Schools/*

## Output Data: `0002_DATA PRODUCTS/`

This folder includes the main outputs generated through the code:
- `schools_exposure.csv` / `.shp`  
  Individual school location and columns indicating yes/no exposure for each hazard. >1.3M rows.

- `countries_exposure.csv`  
  Summary tables by country and hazard

- `countries_SRI.csv` / `.shp`  
  Final School Risk Index and component scores per country

## Dashboard

A summary of the results can be explored here: [SRI Dashboard v2](https://sri-dashboard-v2.onrender.com)