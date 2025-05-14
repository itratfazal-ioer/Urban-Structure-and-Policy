## Step-by-Step Instructions 
Follwing are the steps that can be used to produce training dataset from the building footprint dataset as geopackage in QGIS. 

#### 1. Load Data in QGIS

- Open QGIS and load the **building footprint** layer either as a geopackage or shapefile. 
- Add background reference layers: 
- **Google Satellite imagery** (via XYZ Tiles). should I add our sources for all these layers. 
- **Aerial imagery** 
- **OSM Street Map** (directly from XYZ layer in QGIS)

#### 2. Understand Properties of Categories

- Study the provided building classification schema for each category 
- Understand how each type appears visually in the imagery based on the properties described in schema (e.g., size, shape, position next to other buildings, roof-type structure, neighbourhood, no. of building entrances, etc.).
- Familiarize yourself with the visual properties of each building category 

#### 3. Create a ‘Category’ field 

- In the attribute table of the building footprint feature class/shapefile, create a new text field to add categories of the selected sample buildings.


#### 4. Identify Building Category

- Visually inspection across the imagery to identify buildings and identify structures that clearly reflect the scribed properties of the category. 
Tip: Use 
- Ensure you are selecting buildings from across the entire extent of the study area, not concentrated in one region.

### 5. Assigning Categories 

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
