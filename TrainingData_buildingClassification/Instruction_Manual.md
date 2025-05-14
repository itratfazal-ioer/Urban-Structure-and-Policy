## Step-by-Step Instructions 
Follwing are the steps that can be used to produce training dataset from the building footprint dataset as geopackage in QGIS. These steps were also followed to create training dataset for the building classification as a part of Subdense project. 

#### 1. Load Data in QGIS

- Open QGIS and load the building footprint layer either as a geopackage or shapefile. 
- Add background reference layers: 
  - Google Satellite imagery (via XYZ Tiles). 🔴should I add our sources for all these layers. 
  - Aerial imagery.
  - OSM Street Map (directly from XYZ layer in QGIS).

#### 2. Understand Properties of Categories

- Study the building classification schema defined for the project. Schema document contains a detailed description of each building category. 
- Understand how each type appears visually in the imagery based on the properties described in schema (e.g., size, shape, position next to other buildings, roof-type structure, neighbourhood, no. of building entrances, etc.).
- Familiarize yourself with the visual properties of each building category. 

#### 3. Create a Category field 

- In the attribute table of the building footprint layer, create a new text field where categories of the selected sample buildings will be added. Name it occording to your choice.


#### 4. Identify Building for its Category

- Visually inspect across the imagery to identify buildings that clearly reflect the scribed properties of the category. 
Tip: Use Google Map's 3D Satellite View to determine the category if aerial image layers in QGIS are not helpful enough. Compared to aerial imagery with top-view of buildings only, Google Maps’ 3D Satellite View allows 360° rotation and street-level perspective that can further assist in accurately determining the building’s category.
- Ensure you are selecting buildings from across the entire extent of the study area, not concentrated in one region.

#### 5. Assigning Categories 

- Open the **attribute table** of the building footprint layer.
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
