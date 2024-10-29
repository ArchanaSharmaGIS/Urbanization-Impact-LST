# Urbanization-Impact-LST
## A study on the impact of urbanization on Land Surface Temperature (LST) over two decades in Nagpur District, Maharashtra, using Remote Sensing and GIS technology.


## Table of Contents
- [Project Overview](#project-overview)
- [Motivation](#motivation)
- [Features](#features)
- [Use Cases](#use-cases)
- [Technologies Used](#technologies-used)
- [Data Description](#data-description)
- [Methodology](#methodology)
- [Results](#results)
- [Acknowledgments](#acknowledgments)
## Project Overview
This project analyzes crop drought by leveraging satellite-based remote sensing data and processing it on the Google Earth Engine platform. The core of the analysis focuses on the computation of drought indices (VCI, TCI, and VHI) to visualize and quantify the extent of drought stress on crop vegetation. This project provides key insights for agricultural management, enabling decision-makers to detect early signs of drought stress and implement timely interventions.

## Motivation
With increased frequency of droughts due to climate change, it is critical to monitor crop health and prevent large-scale agricultural losses. Remote sensing data allows for real-time, large-scale monitoring of vegetation health, offering a reliable tool for detecting and mitigating the impact of drought on crop productivity. This project aims to support data-driven agricultural management through accessible and reliable drought monitoring techniques.


## Features
- **Data Retrieval:** Uses Landsat 8 imagery and shapefiles to define the region of interest.
- **Vegetation and Temperature Analysis:** Calculates NDVI-based VCI, LST-based TCI, and combined VHI for drought assessment.
- **Map Visualization:** Displays drought indices on interactive maps for easy visualization.
- **Data Export:** Exports analysis results (VCI, TCI, VHI) as GeoTIFF files.


## Use Cases
- **Agricultural Monitoring**: Identifying drought-stressed regions in agricultural land for early intervention.
- **Drought Assessment**: Provides critical data to aid in governmental and NGO drought relief efforts.
- **Climate Research**: Analyzes the correlation between climate change and drought severity across different regions.

## Technologies Used
- **Google Earth Engine**: For satellite data processing and geospatial analysis.
- **Geemap**: Python package to interact with Google Earth Engine and visualize map outputs.
- **Python**: Core programming language used for data processing and model computation.
- **Landsat 8**: Source of high-resolution spectral data for vegetation and temperature analysis.

## Data Description
This project relies on the following data sources:
- **Landsat 8 Surface Reflectance**: Provides spectral bands used for calculating NDVI.
- **Landsat 8 Thermal Infrared**: Supplies the thermal data needed to compute the Temperature Condition Index.


## Methodology
This project calculates drought indices as follows:
- **NDVI Calculation**: Normalized Difference Vegetation Index is derived from Landsat 8 to monitor vegetation health.
- **VCI Calculation**: Vegetation Condition Index normalizes NDVI to indicate vegetation stress levels.
- **TCI Calculation**: Temperature Condition Index normalizes land surface temperature (LST) to measure thermal stress on vegetation.
- **LST Calculation**: Land Surface Temperature derived from thermal band.
- **VHI Calculation**: Combines VCI and TCI to give an overall Vegetation Health Index, highlighting regions affected by both temperature and vegetation stress.
- **DSI**: Drought Severity Index for evaluating drought conditions.

## Result
- The outputs include GeoTIFF maps of VCI, TCI, and VHI for the specified region. Below is an example interpretation:
- **VCI Map**: Darker colors indicate higher vegetation stress.
- **TCI Map**: Higher TCI values correspond to lower temperature stress.
- **VHI Map**: Combines VCI and TCI, with lower values indicating more severe drought conditions.

### Sample Output:
![Sample VHI Map](output/sample_vhi_map.png)
## Acknowledgments
- **Google Earth Engine**: For the platform and data access.
- **Geemap Library**: For enabling visualization of results on interactive maps.
- **Landsat Data**: Courtesy of the United States Geological Survey (USGS).


