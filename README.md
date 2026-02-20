# wake-county-cemeteries-chavis-clusters

# QGIS
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
 
