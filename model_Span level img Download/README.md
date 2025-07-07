Professional Workflow for Using Automated Models in QGIS for Image Downloading

 1. Adding the Model to the QGIS Processing Toolbox:
   - Open QGIS and navigate to the Processing Toolbox.
   - In the toolbox, find the section labelled Model and load the required model titled with "Image" in its name.
 
 
 2. Preparing the Shapefile for Processing:
   - Import the necessary shapefile into QGIS.
   - Open the attribute table and create a new field with the following specifications:
     - Field Name: `Req_spans`
     - Data Type: Text (String)
     - Length: 80
   - Select the spans you want to process and set the value to 'Yes' in the `Req_spans` column.
 

 3. Importing the Raster Data (GSAT):
   - Import the raster data (e.g., GSAT).
   - Ensure that the coordinate projection of the raster is correctly aligned with the shapefile.


 4. Running the First Model (Req_spans):
   - Select the prepared shapefile and confirm that the projection is accurate.
   - Run the first model, Req_spans.
  - This will generate a temporary buffer file for the selected spans.
   - Review the buffer output for accuracy and hide both the shapefile and buffer file before proceeding to the next step.
 

 5. Executing the Second Model (Img_download):
   - In the Processing Toolbox, open the second model, Img_download, labelled under "Image".
   - Add the output from the first model (buffer file) into the `cloud_polygon_SHP` field.
   - Verify the projection to ensure accuracy.
   - Run the second model. The time taken will vary depending on the file size.
 

 6. Reviewing the Output:
   - Upon completion, the model will output the images for the required spans, ready for further analysis or export.


Output Dataset:
 
Note: “Please ensure that no files are saved as temporary”
