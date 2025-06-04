
## Crop Wild Relative on US Forest Service lands

*Update 2025-06-04*

Major updated based on May meeting. 
- added experimental forests and research natural areas 



1. Utilize the USFS datasets to organize information 
  - layer 1 : Regional areas (9 unique areas)
  - layer 2 : Admin layer (112 unique areas)
  - level 3 : National Forests and Grasslands (260 unique areas)
  - level 4 : Research Natural Areas  (549 unique areas)
  - level 5 : Experimental Forests  (90 unique areas)
  - level 6 : Wilderness Areas (451 unique areas)
  - level 7 : Botanical Areas (46 unique areas)

2. Summarize the total number of species predicted and observed at these areas 
  - predicted : at least a single cell of a habitat suitability model in within the area boundary for a species 
  - observed : at least a single point observation for a specific is found within the area boundary 
  
<div style="display: flex;">
  <div style="flex: 1; padding-right: 10px;">

  <h2>Maps</h2> 
  
  Three maps are generated to so the total predicted and observed species per area
   
   - total taxa ( combined predicted and observed)
   - total taxa observed
   - total taxa predicted  
  <h3>
  <a href= "https://geospatialcentroid.github.io/usfsCWR/combinedMap.html" >Total taxa predicted and observed </a>
  </h3>  
  
  This map looks at the unique taxa between the prediction and observed datasets and provides a full list. This will be the highest number of species of any map. 
  
  <h3>
  <a href= "https://geospatialcentroid.github.io/usfsCWR/pointTaxonMap.html" >Total taxa observed </a>
  </h3>  
  
  This map highlights the number of unique taxa observed within each geography. Every observation indicates a reported ground observation of the species.
  
  <h3>
  <a href= "https://geospatialcentroid.github.io/usfsCWR/predictedTaxonMap.html" >Total taxa predicted </a>
  </h3>  
  
  
  This map highlights the number of unique taxa predicted within each geography. Only a single cell of the potential distribution needs to be in area. 

  </div>
  <div style="flex: 1; padding-left: 10px;">

  <h2>Data summaries </h2>

  Two files were create to summarize the presence of theses species in the specific management areas 
  
  The left move column is the taxon of interest. 
  The column to the right contain the names or unique identifiers of specific forest service areas. 
  
  <h3>
  <a href= "https://docs.google.com/spreadsheets/d/1EDfZUz_WMbgnki1YRBJHVYNkUjlnBknXeHLcnUNw-z8/edit?usp=sharing" >Observed taxa </a>
  </h3>  
  
  <h3>
  <a href= "https://docs.google.com/spreadsheets/d/1AN2E_QwzMjGCo4pj0MWsGOmnDq7wGiq-7bkwibi-x5A/edit?usp=sharing" >Predicted taxa </a>
  </h3>  

  <h2>Area relationship summaries </h2>
  The following files shows the spatial relationship between the various levels of management. Regions, Admin, and National Forest and Grasslands have unique files. 
  The centroid of the largest polygon associate with each area was used to determine the higherachical relationship. 
  
  Assumptions about hierarchy 
  <br>
  Regions : contain (admin, forest and grasslands, research natural areas, experimental forests, wilderness, botanical areas)
  <br>
  Admin : contian (forest and grasslands, research natural areas, experimental forests, wilderness, botanical areas)
  <br>
  forest and grasslands : contain (research natural areas, experimental forests, wilderness, botanical areas)
  
  <h3>
  <a href= "https://docs.google.com/spreadsheets/d/1V9XgBspmeVLLI1C4rY8560JUT4wsk-7bGo2XigsN4TY/edit?usp=sharing" >Regions </a>
  </h3>  
  
  
  <h3>
  <a href= "https://docs.google.com/spreadsheets/d/1wbf1ap1TqvEDlxUwl5ZGCBuJN4ZMqeUGaFr7RHGAN50/edit?usp=sharing" >Admin areas </a>
  </h3>  
  
  <h3>
  <a href= "https://docs.google.com/spreadsheets/d/101kRq3JLdwa1MMMGLdpA8YCGH7LKI1114kZbtMvrQJ0/edit?usp=sharing" >National Forest and Grasslands </a>
  </h3>  
    
  </div>
  
</div>


