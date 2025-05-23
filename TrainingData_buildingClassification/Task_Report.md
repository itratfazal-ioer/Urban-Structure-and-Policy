# Creating Training Data for Building Classification

This document provides a detailed summary on how training data for building classification was produced using building footprint data and reference imagery. For a step-by-step guide, please see the [Instruction Manual](Instruction_Manual.md).


Why doing this task? Purpose? Dataset?
---

## Sampling Methodology

To produce training data from a building footprint dataset, a sample of about 100 buildings was selected for each pre-defined building categories (see Building Classification Schema). Buildings were selected uniformly across the study area, which is critical to avoid spatial bias within the training dataset. However, this approach was not always possible for some categories due to the lack of specific building types in some areas. Despite this, uniform selection was applied as consistently as possible across most categories to maintain the overall spatial representativeness of the dataset.

## Required Inputs

- Building footprint dataset (with existing attribute table)
- Google Satellite imagery - Aerial imagery layer 
- OpenStreetMap (OSM) basemap 
- Building classification schema (e.g., NG_99 = Outbuilding)

## Software Used

- **QGIS** was used to identify and assign building categories to the sample buildings. Any GIS software, such as ArcGIS, can also be used. 

## References
Hecht, Robert. “Automatische Klassifizierung von Gebäudegrundrissen: ein Beitrag zur kleinräumigen Beschreibung der Siedlungsstruktur.” Rhombos-Verlag, 2014. https://www.ssoar.info/ssoar/handle/document/39686.

Hecht, Robert, Gotthard Meinel, and Manfred Buchroithner. “Automatic Identification of Building Types Based on Topographic Databases – a Comparison of Different Data Sources.” International Journal of Cartography 1, no. 1 (January 2, 2015): 18–31. https://doi.org/10.1080/23729333.2015.1055644.







