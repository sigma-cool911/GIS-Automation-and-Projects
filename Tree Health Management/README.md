WORKFLOW

A structured geospatial pipeline was designed to accurately identify and classify dead, partially dead, and unhealthy trees affecting electric infrastructure. The following workflow integrates high-resolution imagery analysis, manual QC, and automated enhancements:

1. Imagery Acquisition & Preprocessing
Used (15-30cm) high-resolution satellite imagery (RGB and/or multispectral).

Filtered and aligned imagery using:

Seasonal consistency

Sun angle normalization

Removal of cloud cover and low-angle artifacts.

2. Initial Tree Health Annotation
Digitized tree-level features based on visual spectral cues:

Color fading (gray, reddish tones)

Loss of canopy structure

Proximity to infrastructure (utility lines, towers)

Mapped as polygons with attribute tree_health:

Dead, Partially Dead, Unhealthy

3. Error Pattern Filtering & Correction
Mitigated the following issues using manual QA + targeted rule sets:

Issue	Correction Strategy
False Positives	Removed shadow-based misclassifications and irrelevant artifacts.
Overprediction	Refined overly large polygons using buffer analysis and neighbor verification.
Color-Based Misclassification	Validated non-green trees against species/type before marking dead.
Vegetation Confusion	Differentiated bushes vs. trees using shape, texture, and context.
Missed Features	Cross-verified small, grey-phase trees using angle-paired imagery.
Polygon Precision	Snapped polygon edges to visible canopy contours; removed overlaps.
Angle Variations	Analyzed imagery from multiple angles to confirm consistency.
Image Shift	Aligned image layers spatially to eliminate positional mismatch.
RGB Band Misinterpretation	Used reference color tables + field insights to validate non-green tones.


4. Health Layer Compilation
Compiled all validated tree polygons into a single shapefile or geopackage.


5. Delivery & Usage
Final layers were exported for use in:

Risk prioritization maps

Vegetation management planning

Model training (e.g., for ML-based detection)


`#QGIS` `#GISAutomation` `#RemoteSensing` `#Python` `#TreeHealth` `#HabitatMapping`  `#SAM` `#CloudPolygon` `#SpanLevel` `#GeospatialAnalysis` `#TreeGrass`
