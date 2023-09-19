# Stinkbug-Geosimulation-System

## Overview

This repo developes an automated, real-time pipeline system to monitor the spread of the Brown marmorated stink bug in Minnesota. The pipeline leverages three distinct models - Gravity, Monte Carlo, and Huff - to simulate the potential dispersion patterns of this invasive species on a monthly basis, based on user-specified input for the year and month.

The automated system processes the output from these models and subsequently uploads the results to a PostGIS database using the shp2pgsql tool. The final map representation of the spread patterns of the stink bug is presented in GeoJSON format and uploaded to ArcGIS Online for easy access and visualization.

In addition, this project employs Google Cloud Run service to host the resulting map layers. This is achieved by utilizing a Dockerfile and requirements file to create a containerized application, ensuring seamless deployment and management of the hosted map layers.

By implementing an automated real-time pipeline system for monitoring the stink bug, this project aims to provide a valuable tool for researchers, policymakers, and stakeholders in Minnesota. It offers insights and data-driven resources to enhance their understanding and management of the invasive species.

## Files
  * **Pipeline_Geosimulation.ipynb**: This script serves as a comprehensive data pipeline, including data fetching, quality assurance and quality control (QAQC), modeling, geo-simulation modeling, and model evaluation.
  * **PostGIS.ipynb**:  This script automates the processes involved in uploading the simulation results to a PostGIS database using the shp2pgsql tool.
  * **app folder**: This directory includes essential files such as the Dockerfile and requirements file, creating a containerized application that utilizes the Google Cloud Run service.

## Output
The repository generates a series of priority maps for stink bug monitoring, which are published on ArcGIS Online for easy access and utilization.

## Author
  * Yaxuan Zhang
  
  * Maochuan Wang
