# Fitzroy River Suspended-Sediment Analysis

Remote sensing analysis of flood-associated relative turbidity in the lower Fitzroy River–estuary, Queensland, using Digital Earth Australia (DEA) Landsat analysis-ready data and river discharge observations.

## Research question

**How did flood and high-flow events influence the spatial extent and relative turbidity of suspended-sediment plumes in the lower Fitzroy River–estuary between 2017 and 2023?**

## Project overview

This project investigates spatial and temporal patterns in suspended-sediment conditions following high-flow events in the Fitzroy River system.

Landsat 8 and 9 observations were analysed in the DEA Sandbox using the Normalised Difference Turbidity Index (NDTI2) as an indicator of relative turbidity. Satellite observations were integrated with Fitzroy River discharge records to compare remotely sensed conditions across background, high, very high and extreme-flow periods.

## Analytical workflow

- Load Landsat 8 and 9 analysis-ready data using Digital Earth Australia
- Apply pixel-quality/cloud masking and a Water Observations from Space (WOfS) water-occurrence mask
- Calculate NDTI2 from red and green reflectance
- Calculate median and 90th-percentile NDTI2 for usable Landsat observations
- Integrate Fitzroy River discharge observations and calculate antecedent-flow metrics
- Classify Landsat observations using discharge percentiles
- Establish pixel-specific background NDTI2 conditions
- Identify areas where event NDTI2 exceeds the local background 90th percentile
- Compare the spatial response between selected high-flow events

## Preliminary findings

The analysis demonstrates substantial variation in the spatial extent of elevated relative turbidity between high-flow events. For example, the area exceeding local background NDTI2 conditions was approximately **144 km² on 21 February 2019** and **248 km² on 30 March 2021**.

These results demonstrate that discharge magnitude alone does not fully describe the spatial expression of elevated turbidity within the estuary.

## Tools and skills

- Python
- Jupyter Notebook
- Digital Earth Australia Sandbox
- xarray and pandas
- Matplotlib
- Landsat remote sensing
- Time-series analysis
- Raster analysis
- QGIS cartography

## Important interpretation

NDTI2 is used here as an indicator of **relative turbidity**, rather than as a direct estimate of total suspended sediment concentration. Elevated areas represent pixels exceeding their location-specific background NDTI2 threshold and should not be interpreted as a definitive physical sediment-plume boundary.

## Project context

This independent portfolio version was developed while studying remote sensing and image analysis. It demonstrates a reproducible Earth observation workflow and does not reproduce assessment instructions, marking criteria, or restricted course materials.

## Data sources

Satellite imagery and derived water products were accessed through Digital Earth Australia. River discharge observations were obtained from the Queensland Water Monitoring Information Portal.
