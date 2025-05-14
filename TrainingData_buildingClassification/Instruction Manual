# Training Data Creation for Building Classification

This document provides a detailed summary and step-by-step guide on how training data for building classification was created using building footprint data and reference imagery.


Why doing this task? Purpose? Dataset?
---

## Overview

To produce training data from a building footprint dataset, a sample of about 100 buildings was selected for each pre-defined building categories (see Building Classification Schema). Buildings were selected uniformly across the study area, which is critical to avoid spatial bias within the training dataset. However, this approach was not always possible for some categories due to the lack of specific building types in some areas. Despite this, uniform selection was applied as consistently as possible across most categories to maintain the overall spatial representativeness of the dataset.

---

## Required Inputs

- Building footprint dataset (with existing attribute table)
- Google Satellite imagery - Aerial imagery layer 
- OpenStreetMap (OSM) basemap 
- Building classification schema (e.g., NG_99 = Outbuilding)
---

## Software Used

- **QGIS** was used to identify and assign building categories to the sample buildings. 

---

## Step-by-Step Instructions

### 1. Load Data in QGIS

- Open QGIS and load the **building footprint** layer either as a geopackage or shapefile. 
- Add background reference layers: 
- **Google Satellite imagery** (via XYZ Tiles). should I add our sources for all these layers. 
- **Aerial imagery** 
- **OSM Street Map** (directly from XYZ layer in QGIS)

### 2. Understand Properties of Categories

- Study the provided building classification schema for each category 
- Understand how each type appears visually in the imagery based on the properties described in schema (e.g., size, shape, position next to other buildings, roof-type structure, neighbourhood, no. of building entrances, etc.).
- Familiarize yourself with the visual properties of each building category 

### 3. Create a ‘Category’ field 

- In the attribute table of the building footprint feature class/shapefile, create a new text field to add categories of the selected sample buildings.


### 3. Identify Building Category

- Visually inspection across the imagery to identify buildings and identify structures that clearly reflect the scribed properties of the category. 
Tip: Use 
- Ensure you are selecting buildings from across the entire extent of the study area, not concentrated in one region.

### 4. Assigning Categories 

- Open the **attribute table** of the building footprint layer.
- Start editting mode.
- At the bottom left of the attribute table window, locate the dropdown "Show All Features" and change it to "Show Selected Features". 
- Now select the building footprint that is identified for a specific category.
- Enter the name of the category in the ‘Category’ field 
- Save your edits.
- Repeat these steps for all other selected sampled buildings

---

## Tips

- Avoid clustered selections; ensure wide spatial coverage.
- Cross-check classification with multiple basemaps for accuracy.
- Categorize only buildings you are confident about.

---

## Output

- A vector file (e.g., GeoPackage or Shapefile) containing category of building footprints ready for use as training data.
