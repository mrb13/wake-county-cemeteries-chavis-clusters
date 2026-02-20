# wake-county-cemeteries-chavis-clusters

# Data Acquisition plan 	

## Findagrave 	

### Cemetery Location 

- Navigate to each cemetery & manually download lat/long details 

### Burial Details 
- search Lastname="Chavis" & Location=Wake County, NC
- Open Chrome DevTools & scroll through all entries
- Identify the proper API calls
- Save JSON outputs manually.  I couldn't figure out how to automate due to anti-automation on server-side 
- save many JSONs to local coputer 

# Data Processing 
- Create new project in VS Code:
	- C:\Users\<user>\Documents\dev\scrape-a-grave-Chavis-WakeCo
python to scrape all burial details
	
# Mapping (QGIS) 
## qgis2web

### Layers & Groups 
- Cemeteries
   - visible=yes
   - popups=yes
      - fields
	   - hidden: cemeteryId, cemeteryName, lat,long
	   - all others: Inline Label - visible with data
Townships
   - visible=yes
   - popups=no
      - fields
	   - hidden: 
	   - all others: Header Label - visible with data
OpenStreet Map
   - visible=yes
   - baseMap=yes

### Appearance
Title: Upper left
Abstract: Upper left
Layers list: Expanded
Attribute Filter: cemeteryName_1
show popups on hover over = yes

### 
Export as Leaflet
 
