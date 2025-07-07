The project follows a hybrid GIS workflow combining AI-powered segmentation (SAM) with manual vector editing in QGIS to extract critical land cover and tree features for Miyawaki forest planning. Below is the structured workflow:

1. Base Imagery Preparation
Acquired high-resolution satellite imagery (e.g., commercial or Sentinel-based RGB composites).

Performed pre-processing (e.g., clipping AOIs, image enhancement if required).

2. Automated Feature Extraction using SAM
Deployed Segment Anything Model (SAM) to generate preliminary object masks:

Extracted individual trees, open plots, and urban features like roads and buildings.

Exported masks as raster or vector layers using Python/QGIS plugins (e.g., Jupyter Notebook + rasterio/geopandas).

3. Post-processing & Manual Refinement
Imported SAM outputs into QGIS for visual inspection.

Performed manual digitization or correction where:

SAM missed small trees or misclassified overlapping features.

4. Land Cover Classification
Classified digitized polygons into meaningful categories:


Vegetation (trees/shrubs)

Barren/Open land

6. Output Generation
Exported final layers:

Cleaned shapefiles (per class)

Attribute-enriched datasets

Ready for integration into urban forestry models, site planning.


`#QGIS` `#GISAutomation` `#RemoteSensing` `#Python` `#TreeHealth` `#HabitatMapping`  `#SAM` `#CloudPolygon` `#SpanLevel` `#GeospatialAnalysis` `#TreeGrass`
