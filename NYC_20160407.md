###<p align="center">**NYC Planimetric Data Descriptions** </p>
#####<p align="center">**NYC DoITT, 2016** </p>

####Purpose<br>
This document provides a summary of each planimetric feature class, including the parameters applied to collect individual features using the latest aerial imagery.

####Introduction<br>
A primary goal of the NYC Citywide GIS is to maintain the accuracy and quality of the base data which includes the orthophotography and planimetrics, collectively known as NYC Map. This base is the foundation upon which virtually all other GIS information within the City of New York is built. Ensuring its completeness and accuracy is fundamental to the Group’s core mission. 
<br><br>
The source imagery was captured on the following dates: <br>• Manhattan - June 24, 2014<br>• The Bronx, Brooklyn, Queens and Staten Island - April 1st through April 25th, 2014<br>• Final delivery of all imagery – April 10, 2015<br><br>Using this orthoimagery, the planimetric base layers were updated citywide starting in March 2015 and were completed in February 2016.

####Table of Contents

&nbsp;&nbsp;&nbsp;&nbsp;[Imagery and Data Specifications](#imagery-and-data-specifications)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[General Attribute Information](#general-attribute-information)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Boardwalk](#boardwalk)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Building Footprints](#building-footprints)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: BUILDING](#subtype-building)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: GARAGE](#subtype-garage)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: BUILDING U/C (Building Under Construction](#subtype-building-uc-building-under-construction)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: SKYBRIDGE](#subtype-skybridge)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Building Footprint Attributes](#building-footprint-attributes)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Building Footprint Diagrams](#building-footprint-diagrams)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Curb](#curb)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Elevation](#elevation)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: BUILDING ELEVATION](#subtype-building-elevation)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: WATER ELEVATION](#subtype-water-elevation)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: SPOT ELEVATION](#subtype-spot-elevation)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: BRIDGE ELEVATION](#subtype-bridge-elevation)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Elevation Attributes](#elevation-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Plaza](#plaza)

<br>
# Imagery and Data Specifications
Digital planimetrics were derived using the imagery products delivered with the 2014 New York Statewide Flyover (see Introduction for specific flight dates), which includes raw imagery collected to support the generation of 0.5 Ft Ground Sample Distance (GSD) natural color imagery. The images were captured with 80% forward lap and side lap to support 1”=100’ mapping and meet the distortion free requirements within New York City. Planimetrics are developed to meet American Society for Photogrammetry and Remote Sensing (ASPRS) Class 1 (one) horizontal mapping standards and ASPRS vertical Class 2 (two) accuracy specifications. Planimetrics are delivered via an ESRI geodatabase in New York State Plane Coordinates, Long Island East Zone, NAD83, US foot.

<br>
# General Attribute Information

The following attribute information applies to all feature classes.  Additional attributes specific to a given feature class are listed within the details for that feature class.

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **Source_ID** | Unique feature Identification Number. |
| **Feature_Code** | Indicates the type of feature.  |
| **Sub_Feature_Code** | (where applicable) indicates a subset of features within a given “Feature_Code” set.  |
| **Status** | Field indicating the feature status as it fits into one of the following categories:<br>a) NEW. A feature captured for the first time during the 2014 planimetrics update project.<br>b) UPDATED. The feature existed previously but has been updated during the 2014 planimetrics update project.<br>c) UNCHANGED. The feature is unchanged from the source planimetrics database. |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# Boardwalk

**Type: Polygon**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | Boardwalks along beachfront. |
| **Capture Notes** | Maintain beach outline/shoreline (do not adjust for tidal differences between imagery flyover dates). |
| **Features Excluded** | n/a | 
| **Feature View** | <p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298093/f0be9c12-fb50-11e5-865c-85d17df0f4ca.png" /></p> |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# Building Footprints

**Type: Polygon**

**Includes the following structures:** [Building](#subtype-building), [Garage](#subtype-garage), [Under Construction Unknown](#subtype-building-uc-building-under-construction), and [Skybridge](#subtype-skybridge)

<br>
### Subtype: BUILDING

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery.<br><br>Used existing building database for reference and for BIN values. For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes). |
| **Features Captured** | All buildings with well-defined walls and roofs that are >400 square feet and taller than 12 feet were captured.<br><br>Buildings with <12 feet height but with BIN were captured.<br><br>Buildings with BIN but <400 square feet were also captured. |
| **Capture Notes** | Buildings with flat roofs were captured on roof outline, capturing the largest outline (excluding overhangs, awnings, construction features, etc.).<br><br>Buildings with pitched roofs were captured on the building footprint.<br><br>Carports, when attached to main building, were included in the outline. Interior divisions within buildings were not captured (used existing building layer and BIN as guide).<br><br>Parcel data and BIN was used as guidance for collection. Where the parcel data indicated that a building should be two or more geometries AND there is NO physical indication, the building was split using the parcel lines. Where the parcel data indicated that a building should be two or more geometries AND there is a physical indication, the building was split using the physical indications. If an existing building was split into several new buildings, the original BIN was retained in only one of the new buildings (ideally the largest) and the new buildings were assigned an "even million" BIN (as a placeholder). BINs can not be duplicated. <br><br>Building Footprints abutting one another on a single tax lot, but each having a unique BIN, were flagged and verified during review.<br><br>If a building was demolished (i.e., as evidenced in the imagery), the BIN was also deleted and was not used for any new building geometry.<br><br>Small triangles denote a permit is out to construct a new building at the location.  These small triangles were added by DoITT building editors. These triangles should be removed when new buildings are added. Therefore if a new building was constructed in the new orthos, the building was captured,  the attributes from triangle to building were transferred to the new building, and the triangle was deleted. If no new building was visible on the orthos, the triangles were left in the data.<br><br>For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes). |
| **Features Excluded** | The following features were not captured:<br>•  temporary trailers, tents, or roofs at gas stations (over pumps).<br>• roofs (overhang) to gas stations, unless connected to building.<br>• movable jet bridge for access to aircraft.<br>• awnings, scaffolds, or sidewalk sheds. | 
| **Feature View** | <p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298164/58700896-fb51-11e5-929f-d0fe4a8c6b7a.png" /></p> |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: GARAGE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery.<br><br>Used existing building database for reference and for BIN values. For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes).<br><br>Used DOF TaxMap as a reference. |
| **Features Captured** | All garages were captured, regardless of size.  To be considered a garage, the structure must have a driveway (paved or unpaved) for road  access, and be able to store one or more cars. |
| **Capture Notes** | Special care was applied to ensure sheds were not confused with garages. In general, standard dimensions for detached garages are approximately 12’x20’ or 14’x20’.<br><br>The Parcel layer was used to place garages within parcel or at parcel boundary – being sure to check for special cases where parcel boundary clearly crosses a garage. In these cases, either the garage was split using physical features, or the property line was used where there was no distinguishing physical feature. |
| **Features Excluded** | Small tool or storage sheds in backyards which have no visible car access were not captured. | 
| **Feature View** | <p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14299040/41289f0e-fb56-11e5-8281-4a2c35073a44.png" /></p> |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BUILDING U/C *(Building under Construction)*

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery.<br><br>The existing DoITT building database was used for reference and for BIN values. For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes). |
| **Features Captured** | Buildings that were under construction in the imagery and had outside walls that clearly indicated the shape of the building were captured. |
| **Capture Notes** |  |
| **Features Excluded** | Under construction buildings were not captured when only the foundation was visible or if the building was being destroyed. | 
| **Feature View** | <p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298827/1767f206-fb55-11e5-985a-51f3679c00cf.png" /></p> |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: SKYBRIDGE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | Elevated walkways that connect buildings were captured as separate building polygons and coded as “Skybridge”. |
| **Capture Notes** | Skybridges were populated with the “HEIGHT_ROOF” attribute only (not Ground Elevation).<br><br>These were assigned an “even million" BIN during capture. For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes). |
| **Features Excluded** |  | 
| **Feature View** | <p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298736/7a7802f6-fb54-11e5-8168-ebae9ac78f7e.png" /></p> |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Building Footprint Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **HEIGHT_ROOF** | Building roof height was calculated as the difference between ground elevation of the building and the roof elevation value.  The roof elevation is the highest point of the roof itself (see BUILDING ELEVATION in the ELEVATION Feature Class). See diagrams below. |
| **GROUND_ELEVATION** | Lowest Elevation at the building ground level.  Calculated from LiDAR or photogrammetrically. |
| **NAME** | pending |
| **BIN** | Building Identification Number.<br><br>In cases where there was no BIN for a building footprint, an "even million” BIN was assigned as follows:<br>• 1000000 for Manhattan,<br>• 2000000 for Bronx,<br>• 3000000 for Brooklyn,<br>• 4000000 for Queens,<br>• 5000000 for Staten Island |
| **CONSTURCTION_YEAR** | Year Built. |
| **GEOM_SOURCE** | pending |
| **LAST_MODIFY_BY** | pending |
| **LAST_MODIFY_DATE** | pending |
| **LAST_STATUS_TYPE** | pending |
| **DOITT_ID** | pending |
| **LAST_STATUS_DATE** | pending |
| **HEIGHT_ROOF** | Elevation at Top of Roof. |
| **DOB_JOB_NUM** | pending |
| **NUM_FLOORS** | Number of Floors. |
| **BUILT_CODE** | pending |
| **COMMENT** | pending |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Building Footprint Diagrams
#####<p align="center">**Calculating HEIGHT_ROOF**</p>

<p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298257/eb233960-fb51-11e5-9db6-a31c1fa23cff.png" /></p>

<p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298243/d95f054c-fb51-11e5-9f00-0a41b3ac3ff3.png" /></p>

<br>
[Back to Table of Contents](#table-of-contents)

<br>
# Curb

**Type: Polyline**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | All curbs between roadbed pavement and other surfaces (i.e., within the street right-of-way) were captured. |
| **Capture Notes** |  |
| **Features Excluded** | Curbs inside Parking lots were not captured. | 
| **Feature View** | <p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298033/959a97b4-fb50-11e5-9f82-d58b82e4516a.png" /></p> |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# Elevation

**Type: Point**

**Includes the following structures:** [Building Elevation](#subtype-building-elevation), [Water Elevation](#subtype-water-elevation), [Spot Elevation](#subtype-spot-elevation), and [Bridge Elevation](#subtype-bridge-elevation)

<br>
### Subtype: BUILDING ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Elevation points were captured for all building footprint features. |
| **Capture Notes** | Elevation of the highest portion of the roof of a building, excluding antennas and roof fixtures such as air conditioning (AC), elevator shafts, chimneys, etc.<br><br>Elevation values were transferred to each building footprint to calculate the building height attribute. |
| **Features Excluded** |  | 
| **Feature View** |  |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: WATER ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Elevation points were captured on standing water (ponds, reservoirs, lakes). |
| **Capture Notes** |  |
| **Features Excluded** |  | 
| **Feature View** |  |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: SPOT ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Spot elevations were captured on paved, unpaved, and alley subtypes in <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> centerline and all <a href="https://data.cityofnewyork.us/dataset/Sidewalk-Centerline/a9xv-vek9/about">Interior Sideswalk CSCL</a> feature classes.  Elevation points were placed in the center of the roadbed (coincident with CSCL features).  These points were captured at the beginning, middle, and end of length of visible roadbed.  Additional elevation points were added at 200’ spacing when the distance between the beginning, middle, or end was greater than 200 linear feet. |
| **Capture Notes** | In areas where the [PAVEMENT_EDGE](#pavement_edge) feature class has been updated, any existing Spot elevations were updated.<br><br>For new streets, new spot elevations were created in the center of the roadbed according to the following rules:<br>1) Placed at Intersections (might not necessarily be at the same location as the node from the centerline, one point per intersection even on complex intersections).<br>2) Placed Every 200 feet when midpoint of bridge or city block exceeds distance.<br>3) Placed on paved, unpaved, alley subtypes in <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> centerline features class and all of the Interior Sidewalk Centerline feature class.  Spot elevation were not added to a CSCL feature if no roadbed exists (e,g, area is under construction).<br>4) Mid-Street segment – at the approximate mid-point of a street segment. |
| **Features Excluded** | Spot elevations were not captured on a <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> feature if no roadbed exists. | 
| **Feature View** |  |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BRIDGE ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** |  |
| **Capture Notes** | This is a subset of spot elevations.  These points were captured at the beginning, middle, and end of length of visible bridges and overpasses.  Additional elevation points were added at 200’ spacing when the distance between the beginning, middle, or end was greater than 200 linear feet. |
| **Features Excluded** | Elevation points were not collected for pedestrian/bike bridges. | 
| **Feature View** |  |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Elevation Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **Elevation** | Field measuring surface elevation above sea level (in feet). |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# Plaza

**Type: Polygon**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | Plazas are hard surfaced "parks" adjacent to public sidewalks or pavement edges. |
| **Capture Notes** | All public space plazas were captured or updated.  Where a plaza is connected to a sidewalk by steps, the steps were considered to be part of the plaza polygon. Planters at the edge of plaza were included as part of the plaza boundary.  Plazas are partitioned from medians and / or sidewalks when adjacent to such features. Walkways within the plaza were captured as part of the overall plaza polygon and were not considered a separate polygon. |
| **Features Excluded** | Private plazas were not captured. | 
| **Feature View** | <p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298127/215672c8-fb51-11e5-9caf-ea052fbfb3f4.png" /></p> |
| **Photo** |  |<br><br>
[Back to Table of Contents](#table-of-contents)
