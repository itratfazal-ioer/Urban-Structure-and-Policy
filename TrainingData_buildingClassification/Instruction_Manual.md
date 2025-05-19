## Instruction Manual 
Following are the steps that can be used to produce training dataset from the building footprint dataset in QGIS. These steps were also followed to create training dataset for the building classification as a part of Subdense project. 


#### 1. Understand Properties of Categories

- Study the building typology defined for the project. Building Typology document contains a detailed description and classification criteria for each building category. Click [here](Building_Typology.md) to see building typology for the SUBDENSE training data task.
- Understand how each type appears visually in the imagery based on the properties described in building typology (e.g., size, shape, position next to other buildings, roof-type structure, neighbourhood, no. of building entrances, etc.).
- Familiarize yourself with the visual properties of each building category.

#### 2. Load Data in QGIS
Now that the typology is understood, classify building footprints into relevant categories. 

- Open QGIS and load the building footprint layer either as a geopackage or shapefile. 
- Add background reference layers: 
  - Google Satellite imagery (via XYZ Tiles). 
  - Aerial imagery.
  - OSM Street Map (directly from XYZ layer in QGIS).

#### 3. Create a Category field 

- In the attribute table of the building footprint layer, create a new text field to store the categories of the selected sample buildings. Name it occording to your choice.


#### 4. Identify Buildings

- Visually inspect across the imagery to identify buildings that clearly match the properties of the category.  
  Tip: Use Google Maps’ 3D Satellite View to determine the category if aerial image layers in QGIS are not helpful enough. Unlike aerial imagery, which offers only the top-view of buildings, Google Maps’ 3D Satellite View allows 360° rotation and street-level perspective that can further assist in accurately determining the building’s category.
- Ensure you are selecting buildings from across the entire extent of the study area, not concentrated in one region.

#### 5. Assigning Categories 

- Open the attribute table of the building footprint layer.
- Start editting mode.
- At the bottom left of the attribute table window, locate the dropdown "Show All Features" and change it to "Show Selected Features". 
- Now select the building footprint that is identified for a specific category.
- Enter the name of the category in the ‘Category’ field 
- Save your edits.
- Repeat these steps for all other selected sampled buildings

---

#### Tips

- Avoid clustered selections; ensure wide spatial coverage.
- Cross-check classification with multiple basemaps for accuracy.
- Categorize only buildings you are confident about.

---

#### Output

- A vector file (e.g., GeoPackage or Shapefile) containing category of building footprints ready for use as training data.
