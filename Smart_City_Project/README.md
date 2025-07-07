1. Data Preparation
Acquired high-resolution satellite imagery and base maps lake regions.

Defined Area of Interest (AOI) covering both lakes and adjacent urban catchments.

2. AI-Assisted Feature Extraction (SAM)
Used Meta’s Segment Anything Model (SAM) to generate vector masks for:

Waterbodies

Invasive vegetation

Islands

Built-up surroundings and shoreline artifacts

Exported masks into QGIS-compatible vector layers for refinement.

3. Manual Digitization & Topology Correction
Reviewed and edited SAM outputs in QGIS to correct:

Partial segmentation of lakes or islands

Manually digitized missing features for full coverage.

4. Attribute Assignment (Smart Framework)
Each spatial feature was assigned values under a structured schema:

Field Name	Description
Unique_ID	Identifier per lake/island feature
Lake_Name	Official waterbody name
Water_Type	Reservoir or canal classification
Catchment	Drainage basin: Northern or Southern
Perimeter	Spatial boundary metric (in meters)
Recreation	Tags for walkways, parks, boating, etc.
Water_Quality_Monitoring	Whether treatment/Wi-Fi float monitoring is enabled
Biodiversity	Key faunal species (e.g., Little Grebes, Painted Storks)
Primary_Source	Inflow source like stormwater or Noyyal River
Label	Classification as Lake or Island

5. Integration for Smart City Use
Merged final shapefile into a centralized QGIS project.

Layer styling based on Catchment, Water_Type, and Biodiversity attributes for rapid decision support.

Prepared geospatial datasets for:

Urban lake rejuvenation planning

Biodiversity conservation (esp. migratory bird zones)

Real-time monitoring via IoT integration

6. Output Delivery
QA-verified shapefiles

Smart attribute tables

Documentation aligned with Smart City policy guidelines.



`#QGIS` `#GISAutomation` `#RemoteSensing` `#Python` `#TreeHealth` `#HabitatMapping`  `#SAM` `#CloudPolygon` `#SpanLevel` `#GeospatialAnalysis` `#TreeGrass`
