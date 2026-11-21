# Exploratory Geospatial Analysis of Recent Changes in Phnom Penh and Kandal Province, Cambodia Using VIIRS Nighttime Lights
This repository contains the Google Earth Engine (GEE) scripts, QGIS template, and research paper for examining urbanization and spatial nighttime light trends across Phnom Penh and Kandal Province, Cambodia from 9/1/2024 to 9/1/2026. The code processes VIIRS Day/Night Band composites to find recent light changes.

<p align="center">
  <img src="https://raw.githubusercontent.com/dariankim/cambodia-viirs-nighttime-lights/main/image results/ROI.png" width="270">
  <img src="https://raw.githubusercontent.com/dariankim/cambodia-viirs-nighttime-lights/main/image results/difference.png"  width="270">
  <img src="https://raw.githubusercontent.com/dariankim/cambodia-viirs-nighttime-lights/main/image results/difference with markers.png" width="270">
</p>
<p align="center"><em> Spatial boundaries of Phnom Penh and Kandal Province shows the region of interest (left), VIIRS nighttime light difference map (center), and annotated difference map highlighting key location and features associated (right).</em></p>

## Paper
**Full Paper:** [Read the PDF](./cambodia_viirs_ntl_analysis.pdf)
* **Key Takeaway:** An exploratory geospaital analysis on recent changes in Phnom Penh and Kandal Province, Cambodia using nighttime lights. By identifying areas with recent nighttime light changes, information on the area, related parties, future urbanization development/land use can be inferred. Limitations such as spatial resolution, temporal resolution, geoblocking, scope, and confirmation bias are discussed for future analysis. 

## Reproducing the Analysis
Script for GEE is available in the "cambodia_viirs_ntl_gee" folder in the file "cambodia_viirs_ntl". Copy and paste all lines of code in this file into an empty file on GEE (including /**** Start of imports... ****/ to reformat imports by hovering over this area). Add shape files under "assets" folder into GEE and fix paths for the associated import variables in the GEE file.

QGIS template for this analysis is available in the "QGIS" folder under "cambodia ntl analysis.qgz". Data layers used are found in the data subfolder. You may need to redirect paths for the data layers. You may also need to zoom into "ROI dissolve" layer in QGIS panel to view the map layers.  

## References
1. Earth Observation Group, Payne Institute for Public Policy, Colorado School of Mines, "VIIRS Nighttime Day/Night Band Composites Version 1", [developers.google.com](https://developers.google.com/earth-engine/datasets/catalog/NOAA_VIIRS_DNB_MONTHLY_V1_VCMCFG#description) 
2. Earth Observation Group, Payne Institute for Public Policy, Colorado School of Mines, "VIIRS Nighttime Light", [eogdata.mines.edu](https://eogdata.mines.edu/products/vnl/)
3. OpenStreetMap contributors, “Relation: Phnom Penh (2199033)”, [openstreetmap.org](https://www.openstreetmap.org/relation/2199033)
4. OpenStreetMap contributors, “Relation: Kandal (2200251)”, [openstreetmap.org](https://www.openstreetmap.org/relation/2200251)
