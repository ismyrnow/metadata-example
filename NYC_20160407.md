###<p align="left">**NYC Planimetric Data Descriptions** </p>

####Purpose<br>
This document is intended to provide a dual purpose. For the capture of the specific planimetric features, this document provides the rules for capture. Under what conditions features are captured, how they are captured and what exceptions apply. Since this document provides a wealth of information that would also benefit users working with the data, we decided to spend a bit more time formatting and presenting this document to further function as a secondary source of documentation. This document is not intended to replace the metadata included with the planimetric features but as a supplement. Lastly, this document orginated from previous planimetric updates that have evolved and been refined over each successive update and will be extended and maintained over the course of future updates.  

####Introduction<br>
A primary goal of the NYC Citywide GIS is to maintain the accuracy and quality of the base data which includes the orthophotography and planimetrics, collectively known as NYC Map. This base is the foundation upon which virtually all other GIS information within the City of New York is built. Ensuring its completeness and accuracy is fundamental to the Group’s core mission. 
<br><br>
The source imagery for the current planimetric update was captured on the following dates: <br>• Manhattan - June 24, 2014<br>• The Bronx, Brooklyn, Queens and Staten Island - April 1st through April 25th, 2014<br>• Final delivery of all imagery – April 10, 2015<br><br>Using this orthoimagery, the planimetric base layers were updated citywide starting in March 2015 and were completed in February 2016.

####Table of Contents

&nbsp;&nbsp;&nbsp;&nbsp;[Imagery and Data Specifications](#imagery-and-data-specifications)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[General Attribute Information](#general-attribute-information)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Boardwalk**](#boardwalk)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Building Footprint**](#building-footprint)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Building](#subtype-building)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Garage](#subtype-garage)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Building U/C (Building Under Construction)](#subtype-building-uc-building-under-construction)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Skybridge](#subtype-skybridge)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Building Footprint Attributes](#building-footprint-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Building Footprint Diagrams](#building-footprint-diagrams)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Curb**](#curb)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Elevation**](#elevation)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Building Elevation](#subtype-building-elevation)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Water Elevation](#subtype-water-elevation)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Spot Elevation](#subtype-spot-elevation)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Bridge Elevation](#subtype-bridge-elevation)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Elevation Attributes](#elevation-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Elevation Diagrams](#elevation-diagrams)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Hydro Structure**](#hydro-structure)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Piers](#subtype-piers)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Jetty](#subtype-jetty)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Seawall](#subtype-seawall)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hydro Structure Attributes](#hydro-structure-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Hydrography**](#hydrography)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Lake/Reservoir](#subtype-lakereservoir)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Pond](#subtype-pond)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: River](#subtype-river)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Stream](#subtype-stream)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Wetland/Marsh](#subtype-wetlandmarsh)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Beach/Shoreline](#subtype-beachshoreline)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Bay/Ocean](#subtype-bayocean)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Hydrography Attributes](#hydrography-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Median**](#median)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Median_Painted](#subtype-median_painted)<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Median_Curb](#subtype-median_curb)<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Median_Rail](#subtype-median_rail)<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Median_Fence](#subtype-median_fence)<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Median_Grass](#subtype-median_grass)<br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Median_Barrier](#subtype-median_barrier)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Median Attributes](#median-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Misc Struct Poly**](#misc-struct-poly)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Billboard](#subtype-billboard)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Sign Gantry](#subtype-sign-gantry)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Toll Plaza](#subtype-toll-plaza)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Misc Struct Poly Attributes](#misc-struct-poly-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Open Space**](#open-space)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Cemetery Outline](#subtype-cemetery-outline)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Recreational Area](#subtype-recreational-area)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Vacant Area](#subtype-vacant-area)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Open Space Attributes](#open-space-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Park**](#park)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Park Boundary](#subtype-park-boundary)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Baseball/Softball Field](#subtype-baseballsoftball-field)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Basketball Court](#subtype-basketball-court)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Handball](#subtype-handball)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Multipurpose Court](#subtype-multipurpose-court)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Tennis Court](#subtype-tennis-court)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Volleyball](#subtype-volleyball)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Football Field](#subtype-football-field)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Soccer Field](#subtype-soccer-field)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Golf Course](#subtype-golf-course)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Pools](#subtype-pools)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Track](#subtype-track)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Skating Rink](#subtype-skating-rink)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Greenstreets](#subtype-greenstreets)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Park Attributes](#park-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Parking Lot**](#parking-lot)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Pavement Edge**](#pavement-edge)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Edge of Pavement](#subtype-edge-of-pavement)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Airport Runway](#subtype-airport-runway)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Alley](#subtype-alley)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Pavement Edge Attributes](#pavement-edge-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Pavement Edge Diagrams](#pavement-edge-diagrams)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Plaza**](#plaza)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Railroad**](#railroad)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Railroad](#subtype-railroad)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Elevated Railroad](#subtype-elevated-railroad)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Embankment Railroad](#subtype-embankment-railroad)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Viaduct Centerline](#subtype-viaduct-centerline)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Depression Railroad](#subtype-depression-railroad)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Railway Fence](#subtype-railway-fence)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Abandoned Railroad](#subtype-abandoned-railroad)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Railroad Attributes](#railroad-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Railroad Structure**](#railroad-structure)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Subway/Train Station](#subtype-subwaytrain-station)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Elevated Subway/Train Station](#subtype-elevated-subwaytrain-station)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Ventilation Grate](#subtype-ventilation-grate)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Emergency Exit](#subtype-emergency-exit)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Transit Entrance](#subtype-transit-entrance)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Railroad Structure Attributes](#railroad-structure-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Retaining Wall**](#retaining-wall)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Retaining Wall](#subtype-retaining-wall)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Railroad Retaining Wall](#subtype-railroad-retaining-wall)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Roadbed**](#roadbed)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Roadbed](#subtype-roadbed)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Intersection](#subtype-intersection)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Driveway](#subtype-driveway)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Shoulder](#subtype-shoulder)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Shoreline**](#shoreline)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Sidewalk**](#sidewalk)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: ROW Sidewalk](#subtype-row-sidewalk)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Interior Sidewalk](#subtype-interior-sidewalk)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Sidewalk Centerline**](#sidewalk-centerline)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Street Furniture Point**](#street-furniture-point)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: City Benches](#subtype-city-benches)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Mailboxes](#subtype-mailboxes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Telephone Booths](#subtype-telephone-booths)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Munimeters](#subtype-munimeters)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Ticket Vending Machines](#subtype-ticket-vending-machines)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Street Seats](#subtype-street-seats)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Street Furniture Poly**](#street-furniture-poly)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Bus Shelters](#subtype-bus-shelters)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Newsstands](#subtype-newsstands)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Automatic Pay Toilet](#subtype-automatic-pay-toilet)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Bike Shelters](#subtype-bike-shelters)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Bike Corral](#subtype-bike-corral)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Planters](#subtype-planters)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Information Kiosks](#subtype-information-kiosks)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Swimming Pool**](#swimming-pool)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Transport Structure**](#transport-structure)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Bridge](#subtype-bridge)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Tunnel](#subtype-tunnel)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Rail Bridge](#subtype-rail-bridge)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Pedestrian/Bike Bridge](#subtype-pedestrianbike-bridge)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Railroad Viaduct](#subtype-railroad-viaduct)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: Overpass](#subtype-overpass)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Transport Structure Attributes](#transport-structure-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**Under Construction Unknown**](#under-construction-unknown)

<br>
# Imagery and Data Specifications
Digital planimetrics were derived using the imagery products delivered with the 2014 New York Statewide Flyover (see Introduction for specific flight dates), which includes raw imagery collected to support the generation of 0.5 Ft Ground Sample Distance (GSD) natural color imagery. The images were captured with 80% forward lap and side lap to support 1”=100’ mapping and meet the distortion free requirements within New York City. Planimetrics are developed to meet American Society for Photogrammetry and Remote Sensing (ASPRS) Class 1 (one) horizontal mapping standards and ASPRS vertical Class 2 (two) accuracy specifications. Planimetrics are delivered via an ESRI geodatabase in New York State Plane Coordinates, Long Island East Zone, NAD83, US foot.

<br>
# General Attribute Information

The following attribute information applies to all feature classes.  Additional attributes specific to a given feature class are listed within the details for that feature class.

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **SOURCE_ID** | Unique feature Identification Number. |
| **FEATURE_CODE** | Indicates the type of feature.  |
| **SUB_FEATURE_CODE** | (where applicable) indicates a subset of features within a given “Feature_Code” set.  |
| **STATUS** | Field indicating the feature status as it fits into one of the following categories:<br>a) NEW. A feature captured for the first time during the 2014 planimetrics update project.<br>b) UPDATED. The feature existed previously but has been updated during the 2014 planimetrics update project.<br>c) UNCHANGED. The feature is unchanged from the source planimetrics database. |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# BOARDWALK

**Geometry Type: Polygon**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | Boardwalks along beachfront. |
| **Capture Notes** | Maintain beach outline/shoreline (do not adjust for tidal differences between imagery flyover dates). |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14476692/58a7b27e-00d7-11e6-98d1-c4c985301f02.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# BUILDING FOOTPRINT

**Geometry Type: Polygon**

**Includes the following structures:** [Building](#subtype-building), [Garage](#subtype-garage), [Under Construction Unknown](#subtype-building-uc-building-under-construction), and [Skybridge](#subtype-skybridge)

<br>
### Subtype: BUILDING

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery.<br><br>Used existing building database for reference and for BIN values. For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes). |
| **Features Captured** | All buildings with well-defined walls and roofs that are >400 square feet and taller than 12 feet were captured.<br><br>Buildings with <12 feet height but with BIN were captured.<br><br>Buildings with BIN but <400 square feet were also captured. |
| **Capture Notes** | Buildings with flat roofs were captured on roof outline, capturing the largest outline (excluding overhangs, awnings, construction features, etc.).<br><br>Buildings with pitched roofs were captured on the building footprint.<br><br>Carports, when attached to main building, were included in the outline. Interior divisions within buildings were not captured (used existing building layer and BIN as guide).<br><br>Parcel data and BIN was used as guidance for collection. Where the parcel data indicated that a building should be two or more geometries AND there is NO physical indication, the building was split using the parcel lines. Where the parcel data indicated that a building should be two or more geometries AND there is a physical indication, the building was split using the physical indications. If an existing building was split into several new buildings, the original BIN was retained in only one of the new buildings (ideally the largest) and the new buildings were assigned an "even million" BIN (as a placeholder). BINs can not be duplicated. <br><br>Building Footprints abutting one another on a single tax lot, but each having a unique BIN, were flagged and verified during review.<br><br>If a building was demolished (i.e., as evidenced in the imagery), the BIN was also deleted and was not used for any new building geometry.<br><br>Small triangles denote a permit is out to construct a new building at the location.  These small triangles were added by DoITT building editors. These triangles should be removed when new buildings are added. Therefore if a new building was constructed in the new orthos, the building was captured,  the attributes from triangle to building were transferred to the new building, and the triangle was deleted. If no new building was visible on the orthos, the triangles were left in the data.<br><br>For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes). |
| **Features Excluded** | The following features were not captured:<br>•  temporary trailers, tents, or roofs at gas stations (over pumps).<br>• roofs (overhang) to gas stations, unless connected to building.<br>• movable jet bridge for access to aircraft.<br>• awnings, scaffolds, or sidewalk sheds. | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298164/58700896-fb51-11e5-929f-d0fe4a8c6b7a.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: GARAGE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery.<br><br>Used existing building database for reference and for BIN values. For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes).<br><br>Used DOF TaxMap as a reference. |
| **Features Captured** | All garages were captured, regardless of size.  To be considered a garage, the structure must have a driveway (paved or unpaved) for road  access, and be able to store one or more cars. |
| **Capture Notes** | Special care was applied to ensure sheds were not confused with garages. In general, standard dimensions for detached garages are approximately 12’x20’ or 14’x20’.<br><br>The Parcel layer was used to place garages within parcel or at parcel boundary – being sure to check for special cases where parcel boundary clearly crosses a garage. In these cases, either the garage was split using physical features, or the property line was used where there was no distinguishing physical feature. |
| **Features Excluded** | Small tool or storage sheds in backyards which have no visible car access were not captured. | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14299040/41289f0e-fb56-11e5-8281-4a2c35073a44.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BUILDING U/C *(Building under Construction)*

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery.<br><br>The existing DoITT building database was used for reference and for BIN values. For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes). |
| **Features Captured** | Buildings that were under construction in the imagery and had outside walls that clearly indicated the shape of the building were captured. |
| **Capture Notes** | n/a |
| **Features Excluded** | Under construction buildings were not captured when only the foundation was visible or if the building was being destroyed. | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298827/1767f206-fb55-11e5-985a-51f3679c00cf.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: SKYBRIDGE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | Elevated walkways that connect buildings were captured as separate building polygons and coded as “Skybridge”. |
| **Capture Notes** | Skybridges were populated with the “HEIGHT_ROOF” attribute only (not Ground Elevation).<br><br>These were assigned an “even million" BIN during capture. For more information regarding BIN, see [Building Footprint Attributes](#building-footprint-attributes). |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298736/7a7802f6-fb54-11e5-8168-ebae9ac78f7e.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Building Footprint Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **HEIGHT_ROOF** | Building roof height was calculated as the difference between ground elevation of the building and the roof elevation value.  The roof elevation is the highest point of the roof itself (see [BUILDING ELEVATION](#subtype-building-elevation) in the [ELEVATION](#elevation) Feature Class). See [Building Footprint Diagrams](#building-footprint-diagrams) below for additional details. |
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
# CURB

**Geometry Type: Polyline**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | All curbs between roadbed pavement and other surfaces (i.e., within the street right-of-way) were captured. |
| **Capture Notes** | This is a new feature class in the 2014 collection.  Prior to the 2014 capture, Curbs were a subset of the Pavement Edge feature class but have been broken out into a seperate feature class in 2014. |
| **Features Excluded** | Curbs inside Parking lots were not captured. | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298033/959a97b4-fb50-11e5-9f82-d58b82e4516a.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# ELEVATION

**Geometry Type: Point**

**Includes the following elevation sites:** [Building Elevation](#subtype-building-elevation), [Water Elevation](#subtype-water-elevation), [Spot Elevation](#subtype-spot-elevation), and [Bridge Elevation](#subtype-bridge-elevation)

<br>
### Subtype: BUILDING ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Elevation points were captured for all building footprint features. |
| **Capture Notes** | Elevation of the highest portion of the roof of a building, excluding antennas and roof fixtures such as air conditioning (AC), elevator shafts, chimneys, etc.<br><br>Elevation values were transferred to each building footprint to calculate the building height attribute. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: WATER ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Elevation points were captured on standing water (ponds, reservoirs, lakes). |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: SPOT ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Spot elevations were captured on paved, unpaved, and alley subtypes in <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> centerline and all <a href="https://data.cityofnewyork.us/dataset/Sidewalk-Centerline/a9xv-vek9/about">Interior Sideswalk CSCL</a> feature classes.  Elevation points were placed in the center of the roadbed (coincident with CSCL features).  These points were captured at the beginning, middle, and end of length of visible roadbed.  Additional elevation points were added at 200’ spacing when the distance between the beginning, middle, or end was greater than 200 linear feet. |
| **Capture Notes** | In areas where the [PAVEMENT_EDGE](#pavement_edge) feature class has been updated, any existing Spot elevations were updated.<br><br>For new streets, new spot elevations were created in the center of the roadbed according to the following rules:<br>1) Placed at Intersections (might not necessarily be at the same location as the node from the centerline, one point per intersection even on complex intersections).<br>2) Placed Every 200 feet when midpoint of bridge or city block exceeds distance.<br>3) Placed on paved, unpaved, alley subtypes in <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> centerline features class and all of the Interior Sidewalk Centerline feature class.  Spot elevation were not added to a CSCL feature if no roadbed exists (e,g, area is under construction).<br>4) Mid-Street segment – at the approximate mid-point of a street segment. |
| **Features Excluded** | Spot elevations were not captured on a <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> feature if no roadbed exists. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BRIDGE ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | n/a |
| **Capture Notes** | This is a subset of spot elevations.  These points were captured at the beginning, middle, and end of length of visible bridges and overpasses.  Additional elevation points were added at 200’ spacing when the distance between the beginning, middle, or end was greater than 200 linear feet. |
| **Features Excluded** | Elevation points were not collected for pedestrian/bike bridges. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Elevation Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **Elevation** | Field measuring surface elevation above sea level (in feet). |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Elevation Diagrams

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14506728/3ebc111e-018d-11e6-979b-5f5049aaf392.png" /></p>

[Back to Table of Contents](#table-of-contents)

<br>
# HYDRO STRUCTURE

**Geometry Type: Polygon**

**Includes the following structures:** [Piers](#subtype-piers), [Jetty](#subtype-jetty), and [Seawall](#subtype-seawall)

<br>
### Subtype: PIERS

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Decks supported by posts extending into the water. |
| **Capture Notes** | Updated piers, commercial piers, and docks. Used existing plnimetrics data as guide. |
| **Features Excluded** | Individual/private docks for recreational watercraft were not captured, unless they had already been captured as such in existing planimetric data. | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14507708/f8cc1802-0191-11e6-9ec6-9677ab053f89.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: JETTY

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Structures, usually comprised of stone, earth, or concrete, extending from shore to lessen erosion.  They are often installed in continuation of river channels at their outlets or into docks, and outside their entrances. |
| **Capture Notes** | Delineated at the water level. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14507754/3831db44-0192-11e6-92bb-8328aadffd95.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: SEAWALL

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Seawalls are typically built on the land parallel to the coast, but may also include breakwaters that are built into the water. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14507849/a98c2d94-0192-11e6-9c4e-1d8dfcf3d475.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Hydro Structure Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **Elevation** | Field measuring surface elevation above sea level (in feet). |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# HYDROGRAPHY

**Geometry Type: Polygon**

**Includes the following features:** [Lake/Reservoir](#subtype-lake/reservoir), [Pond](#subtype-pond), [River](#subtype-river), [Stream](#subtype-stream), [Wetland/Marsh](#subtype-wetland/marsh), [Beach/Shoreline](#subtype-beach/shoreline), and [Bay/Ocean](#subtype-bay/ocean)

<br>
### Subtype: LAKE/RESERVOIR

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | n/a |
| **Capture Notes** | Updated all Lake/Reservoirs when general shape had changed. Existing features were not updated due to different water level. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14507956/308f5492-0193-11e6-9432-2197f04247ea.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: POND

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | n/a |
| **Capture Notes** | Updated pond outline when general shape had changed. Existing features were not updated due to different water level. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14507981/52461954-0193-11e6-81cb-1276596d5f16.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: RIVER

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | n/a |
| **Capture Notes** | Updated all river whenever new conditions were encountered (e.g., due to piers, etc.).  Maintained internal divisions of river due to name change(s). |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508022/90d794e0-0193-11e6-9e9c-3e5ca896aa1e.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: STREAM

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | n/a |
| **Capture Notes** | Updated all streams found to be wider than eight (8) feet if bank had changed.  Maintained internal divisions of stream due to name change(s). |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508065/c76737c2-0193-11e6-9c23-d545c3f871ef.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: WETLAND/MARSH

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | n/a |
| **Capture Notes** | Update wetland and marsh boundaries only when changed due to drainage, change in surface, or if covered by buildings. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508172/3c69c3be-0194-11e6-9642-d27e8c80aff4.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BEACH/SHORELINE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | n/a |
| **Capture Notes** | Updated beach and shoreline whenever feature had changed due to construction or erosion.  DoITT designation in existing files was maintained. Maintained interior divisions.  Did not update due to different water level (high/low tide). |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508219/6d58c4c0-0194-11e6-9898-6d644ae69da7.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BAY/OCEAN

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | n/a |
| **Capture Notes** | Updated bay/ocean shoreline whenever feature had changed due to construction or erosion.  DoITT designation in existing files was maintained. Maintained interior divisions.  Did not update due to different water level (high/low tide). |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508272/b0e93bac-0194-11e6-8089-3706bee67d14.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Hydrography Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **NAME** | Name of Waterbody or Watercourse. |<br><br>

[Back to Table of Contents](#table-of-contents)

<br>
# MEDIAN

**Geometry Type: Polygon**

**Includes the following features:** [Median_Painted](#subtype-median_painted), [Median_Curb](#subtype-median_curb), [Median_Rail](#subtype-median_rail), [Median_Fence](#subtype-median_fence), [Median_Grass](#subtype-median_grass), and [Median_Barrier](#subtype-median_barrier)

<br>
### General Guidelines for Medians

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | All medians that physically divide a roadbed were collected, which include medians, traffic islands, "Jersey Barriers", and painted areas that are used to separate the traffic flow. |
| **Capture Notes** | Medians are sometimes paved, are normally elevated (have a curb), or may have dirt or grass.<br><br>Medians can have sidewalks crossing them. In those cases, the outline of the largest area was incorporated into a single median feature.<br><br>The NYC online Bike Lane data was used as a reference to identify potential new medians. Areas where the column ALLCLASSES is equal to I and "I,II" most often contained new medians. New Medians exist throughout the City regardless of these bike lane classifications. Thus, this was considered a supplemental source only. |
| **Features Excluded** | The following features were not captured as medians:<br>&nbsp;&nbsp;&nbsp;• Barriers in front of buildings,<br>&nbsp;&nbsp;&nbsp;• Jersey Barriers used to regulate traffic in construction areas, or<br>&nbsp;&nbsp;&nbsp;• Jersey Barriers used to block-off road access. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: MEDIAN_PAINTED

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Medians having white paved marking (fishbone or striped pattern). |
| **Capture Notes** | n/a |
| **Features Excluded** | Double yellow lines in the middle of a road were not captured as median.<br><br>Single independent white medians hatching used to direct traffic were not captured as median. | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508345/fec96248-0194-11e6-8e2f-030a7da9874a.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: MEDIAN_CURB

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Medians with curb edging, regardless of interior content (grass, pavement, concrete, etc.). |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508428/64b8b19e-0195-11e6-89fd-9a074b7c4b30.png" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: MEDIAN_RAIL

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Medians with guardrail outlining the curb of the median.  |
| **Capture Notes** | These features incorporate a fixed width of three (3) feet centered on the fence. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508473/960a7b38-0195-11e6-8cc7-a4ba51b33e73.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: MEDIAN_FENCE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Medians with fencing.   |
| **Capture Notes** | n/a |
| **Features Excluded** | If feature respresents a Jersey Barrier with fencing, the feature was collected as a Jersey barrier. | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508506/b6c83cde-0195-11e6-8ec7-83bebee5e1fa.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: MEDIAN_GRASS

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Medians with grass/vegetation inside and no curb. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508545/e48450c2-0195-11e6-9d9b-b3c58dce9a7b.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: MEDIAN_BARRIER

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | "Jersey barriers" of a “permanent nature” (i.e., in place to regulate the traffic, positioned at a constant width of three (3) feet centered on the barrier).  |
| **Capture Notes** | Whenever two jersey barriers were placed next to or in short distance of each other, the outer-most edge of both were used to determine the outline of a single feature. |
| **Features Excluded** | Barrier medians which are moved on a daily basis, (e.g., at Manhattan entrances to Lincoln Tunnel) were not captured. | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14508618/55072680-0196-11e6-909c-c9a1ca19529a.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Median Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **STREET_NAME** | pending |<br><br>

[Back to Table of Contents](#table-of-contents)

<br>
# MISC STRUCT POLY

**Geometry Type: Polygon**

**Includes the following structures:** [Billboard](#subtype-billboard), [Sign Gantry](#subtype-sign-gantry), and [Toll Plaza](#subtype-toll-plaza)

<br>
### Subtype: BILLBOARD

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | All billboards (including those found on rooftops), with three foot standard width. |
| **Capture Notes** | These features are represented with multiple shapes (triangle, V- shaped, etc.). |
| **Features Excluded** | Support structures were not included as part of these features. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: SIGN GANTRY

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Traffic information strutures that cross traffic lanes. |
| **Capture Notes** | These features were digitized end-to-end, with seven foot standard width. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: TOLL PLAZA

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Roof outline of toll plaza buildings (tool booths), regardless of size. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Misc Struct Poly Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **DESCRIPTION** | Field characterizing the miscellaneous structure. |<br><br>

[Back to Table of Contents](#table-of-contents)

<br>
# OPEN SPACE

**Geometry Type: Polygon**

**Includes the following structures:** [Cemetery Outline](#subtype-cemetery-outline), [Recreational Area](#subtype-recreational-area), and [Vacant Area](#subtype-vacant-area)

<br>
### Subtype: CEMETERY OUTLINE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated cemetery boundaries from new imagery. |
| **Capture Notes** | Individual headstones, graves, or interior boundaries were not partitioned. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: RECREATIONAL AREA

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Outline of recreational areas which may be used for picnic or other recreational activities. Recreational areas must contain at least one of the following:<br>&nbsp;&nbsp;&nbsp;a) Benches,<br>&nbsp;&nbsp;&nbsp;b) Swings, or<br>&nbsp;&nbsp;&nbsp;c) Play area<br><br>Hardscape recreation areas were collected differently than softscape recreational areas, as follows:<br><br>• Hardscape recreational areas have either hard surfaces or sand. These areas were captured as discrete polygons following the edges of these areas precisely.<br><br>• Softscape recreational areas are grassy areas for football/baseball/other. These areas were captured as a single polygon (i.e., not discrete polygons) and snapped to other features (e.g. sidewalks, roadbed, hydro, etc.) where applicable.<br><br>When hardscapes and softscapes exists adjacent to one another, the entire area was captured by a single polygon. |
| **Capture Notes** | These features are entirely outside the limits of NYC designated parks. Instead, these include areas such as Brooklyn Bridge Park and the High Line. |
| **Features Excluded** | Medians with either benches, swings, or play areas were captured as a median and not a recreational area. |
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: VACANT AREA

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing data Digital Tax Map (DTM). |
| **Features Captured** | These features represent a vacant lot where a building could potentially be built and is associated with a tax lot polygon. |
| **Capture Notes** | "Vacant" is defined herein as an area containing no structures.<br><br>The DTM and currently captured planimetrics ([Building Footprints](#building-footprints)) were used to determine the location of the vacant areas.<br><br>The actual shape of each vacant aras was captured using physical features that typically form the boundary of a property such as fences, hedgerow, etc.<br><br>Vacant Areas extend to sidewalk or roadbed edge. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Open Space Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **NAME** | Name of Open Space Area. |<br><br>

[Back to Table of Contents](#table-of-contents)

<br>
# PARK

**Geometry Type: Polygon**

**Includes the following structures:** [Park Boundary](#subtype-park-boundary), [Baseball/Softball Field](#subtype-baseballsoftball-field), [Basketball Court](#subtype-basketball-court), [Handball](#subtype-handball), [Multipurpose Court](#subtype-multipurpose-court), [Tennis Court](#subtype-tennis-court), [Volleyball](#subtype-volleyball), [Football Field](#subtype-football-field), [Soccer Field](#subtype-soccer-field), [Golf Course](#subtype-golf-course), [Pools](#subtype-pools), [Track](#subtype-track), [Skating Rink](#subtype-skating-rink), and [Greenstreets](#subtype-greenstreets)

<br>
### Subtype: PARK BOUNDARY

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline the outer perimeter of any park from <a href="https://data.cityofnewyork.us/City-Government/Parks-Properties/rjaj-zgq7/about">DPR Parks Properties</a>.<br><br>The boundary encompasses the entire park as a single polygon feature, regardless of special features such as baseball diamonds or tennis courts.<br><br>The delineation of the outer edge of each park boundary is coincident with the “intended” boundary feature, as determined by the Parks Department. Intended boundary feature are curbs, green areas, sidewalks, etc. and vary from park to park.  At times, the intended boundary feature varies within the same park.  |
| **Capture Notes** | When the source data had a single boundary polygon extending across other planimetric features (e.g. roads), the planimetric park boundary follows the source data.<br><br>When there was no apparent physical boundary feature to delineate the Park boundary, the feature was copied “as is” from the source database.<br><br>Park names (SIGNNAME and source column) and park numbers (GISPROPNUM source column) were transferred from source databases to park boundaries and special features.<br><br>Interior road systems and special features within parks were not partitioned. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BASEBALL/SOFTBALL FIELD

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of the sandy area (diamond) in softball/baseball fields. |
| **Capture Notes** |  These features can have different sizes and can be also be represented as painted areas on hard surfaces.<br><br>These features extend back to the backstop of the field and include the 1st and 3rd base coaching boxes. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BASKETBALL COURT

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of individual basketball courts. |
| **Capture Notes** |  These features can be represented as full or half courts. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: HANDBALL

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of handball courts. |
| **Capture Notes** | The hard surface wall was incorporated witin each court. When multiple courts are adjacent to one another, a  division line was digitized to partition individual courts. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: MULTIPURPOSE COURT

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of multipurpose fields. |
| **Capture Notes** |  These features are composed of mostly hard surface areas with different markings for different activities. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: TENNIS COURT

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of tennis courts (hard surface only). |
| **Capture Notes** | In cases of multiple courts, a division line was digitized along outer painted line (baseline and sideline) to partition individual courts.<br><br>The extent of these features only includes "in-bounds areas", they do not extend to the fence surrounding the tennis court area (or related "out-of-bounds areas". |
| **Features Excluded** | Tennis courts within NYC Parks were not captured.<br><br>Private tennis courts (e.g., on roofs of hotels, etc.) were not captured. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: VOLLEYBALL

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of volleyball courts using distinct markings on observed hard surface. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: FOOTBALL FIELD

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of football fields. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: SOCCER FIELD

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of soccer fields. |
| **Capture Notes** |  Outline is represent by extent of grassy surface. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: GOLF COURSE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of golf courses along fence or other man-made boundary. |
| **Capture Notes** | n/a |
| **Features Excluded** | The outline of greens, tees, fairways, sand traps, shelters, or cart paths were not captured. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: POOLS

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of public pool areas. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: TRACK

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of running tracks, typically around grassy sport fields. |
| **Capture Notes** | n/a |
| **Features Excluded** | Tracks painted upon concrete surfaces were not captured. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: SKATING RINK

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Outline of skating/hockey rinks using distinct markings on observed hard surface. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: GREENSTREETS

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Using <a href="https://data.cityofnewyork.us/Environment/Greenstreets/p23h-ci72">DPR Greenstreets</a> as the definitive source, these areas were updated and attributed using the source data. Name was populated from the SITENAME source column and park numbers were populated from the GISPROPNUM source column. |
| **Capture Notes** | All the rules for defining park boundaries were applied for defining Greenstreet limits. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Park Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **PARK_NAME** | pending |
| **PARKNUM** | Unique park identification number corresponding with PARK_NAME. |
| **SYSTEM** | pending |
| **LANDUSE** | pending |<br>

[Back to Table of Contents](#table-of-contents)

<br>
# PARKING LOT

**Geometry Type: Polygon**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | All parking lots (paved or unpaved) greater than 2,000 sq. feet.<br><br>Parking areas adjacent to the travel-way and separated from the travel-way by a curb or other obstruction were captured as parking lots. In these cases, the [Roadbed](#roadbed) and [Pavement Edge](#pavement-edge) end or wrap around the parking lot. The parking lot is not included as part of the Roadbed. |
| **Capture Notes** | These features connect to road edge ([Curb](#curb) or [Edge of Pavement](#subtype-edge-of-pavement)) only at entrances and exits. |
| **Features Excluded** | Traffic islands within parking lot were not captured.<br><br>When a building of > 400 sq. feet was present, the building area was excluded from the parking lot polygon.<br><br>Parking areas adjacent to the travel-way, but not separated from the travel-way by a curb or other obstruction, were not captured.  Instead, those parking areas were included as part of the Roadbed and the Pavement Edge extends to the outside edge of such area.  | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# PAVEMENT EDGE

**Geometry Type: Polyline**

**Includes the following structures:** [Edge Of Pavement](#subtype-edge-of-pavement), [Airport Runway](#subtype-airport-runway), and [Alley](#subtype-alley)

<br>
### Subtype: EDGE OF PAVEMENT

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | Updated all segments between pavement and other surfaces or features (i.e. Curbs, sidewalks, or grass).  |
| **Capture Notes** | Each segment was captured as a continuous feature across a blockface (typically from one intersection to the next – along that side of the road). <br><br>The vertex between two segments was often located at the street corner. Edge of Pavement features are continuous across driveways, alleys, or access to parking. The one exception to this rule is where a street segment changes names (as determined by <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> Centerline names) outside of any street intersections.  In these cases, the existing CSCL break (node) was used to create corresponding breaks in Pavement Edge segments.<br><br>For cul-de-sacs, two segments were created. The CSCL centerline was used to define the breakpoints of the Pavement Edge segments.<br><br>Dead end streets were terminatde where the tax map crosses the road.  Two segments were created on left and right sides of CSCL.<br><br>On highways, Pavement Edge corresponds to the ‘roadbed’ sub-feature class in [Roadbed](#roadbed), and does not include the shoulder. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: AIRPORT RUNWAY

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | The outer-edge of all paved features associated with airports, including runways, taxiways and aprons. |
| **Capture Notes** | The features often share an edge with a building feature. Airport features were collected up to the surrounding fence or gates. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: ALLEY

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery, existing planimetrics, and Parks database. |
| **Features Captured** | These features represent a narrow unnamed street that allows access to buildings/garages other than from the road. When captured, these features were snapped to the road edge. |
| **Capture Notes** | These feature typically allow access to the interior of a block or to the back of a house.  As a general rule of thumb, the <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> value of: RW_TYPE=10 was used to determine the alley pavement edge.  However, there were still alleys captured that did not have this field attribute value from the CSCL. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Pavement Edge Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **BLOCKFACEID** | Field indicates the Unique ID generated automatically.<br><br>This ID was conflated to the corresponding L/R BLOCKFACEID in <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a>.<br><br>See [Pavement Edge Diagrams](#pavement-edge-diagrams) for more details on conflation with special/complex scenarios. |<br><br>
| **CONFLATED** | Field indicates whether or not the BLOCKFACEID value was conflated to a CSCL segment.<br><br>Values are Y or N. |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Pavement Edge Diagrams

This section includes the following capture rules pertaining to BlockfaceID conflation from Pavement Edge to <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> for these special/complex cases:<br>
1. [Capture Rule for missing CSCL](#1-blockfaceid-conflation-from-pavement-edge-to-cscl---rule-for-missing-cscl)<br>
2. [Capture Rule for Medians](#2-blockfaceid-conflation-from-pavement-edge-to-cscl---rules-for-medians)<br>
3. [Capture Rule for Multiple CSCL with Single Pavement Edge](#3-blockfaceid-conflation-from-pavement-edge-to-cscl----rule-for-multiple-cscl-segments-with-a-single-pavement-edge)<br>
4. [Capture Rule for Multiple PavementEdge with single CSCL segment](#4-blockfaceid-conflation-from-pavement-edge-to-cscl---rule-for-multiple-pavement-edge-with-single-cscl-segment)<br>
5. [Capture Rule for handling complex intersection/median/bridge scenarios](#5-blockfaceid-conflation-from-pavement-edge-to-cscl---rule-for-handling-complex-intersectionmedianbridge-scenarios)

<br>
#####1. BlockfaceID conflation from Pavement Edge to CSCL - Rule for missing CSCL

• If no <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> feature existed on an existing roadbed with Pavement Edge, the production team broke down the Pavement Edge as needed on the approximated center of where a CSCL Centerline and then assigned L/R BlockfaceIDs to the Pavement Edge.  However, these BlockfaceIDs were not conflated to any CSCL segments (and these Pavement Edge features were flagged as having a BlockfaceID that was not conflated to CSCL).<br>

**The following are examples of where CSCL is missing and PavementEdge exists.**

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14505360/d0d2e606-0186-11e6-9b27-1530a2e06280.png" /></p>
<br>
<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14505398/f180e8bc-0186-11e6-8381-baa29da52def.png" /></p>

[Back to Table of Contents](#table-of-contents)

<br>

#####2. BlockfaceID conflation from Pavement Edge to CSCL - Rules for Medians

• When a <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> segment is bounded on one or both sides by a median, the longest edges of median Pavement Edge was assigned BlockfaceIDs, which were conflated onto applicable adjacent CSCL segments.<br>
• Assigned BlockfaceIDs to Pavement Edge for all medians except painted medians.<br>
• Conflated to CSCL where no Pavement Edge derived BlockfaceID takes priority, and there was a CSCL segment that corresponds to the long edge of the median.<br>
• In cases where medians are within medians, the conflating median is the majority (containing) median.<br>
• Pavement Edge features on a median were flagged as having a BlockfaceID that was not conflated to CSCL.<br>

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14505677/31b4ee6e-0188-11e6-900a-9890644e6a0a.png" /></p>
<br>
<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14506419/bd97e6e0-018b-11e6-9ff4-4fd4308dad0d.png" /></p>
<br>
<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14506424/c4c0a66e-018b-11e6-90e1-06163cb23cba.png" /></p>

[Back to Table of Contents](#table-of-contents)

<br>

#####3. BlockfaceID conflation from Pavement Edge to CSCL -  Rule for Multiple CSCL Segments with a Single Pavement Edge

• In cases where there are multiple <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> segments running along a single Pavement Edge (median or otherwise), the BlockfaceID from the Pavement Edge was conflated to the CSCL segments that correspond to the single Pavement Edge.<br>

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14506127/4d80901a-018a-11e6-88c8-aa2a60bddb17.png" /></p>

[Back to Table of Contents](#table-of-contents)

<br>

#####4. BlockfaceID conflation from Pavement Edge to CSCL - Rule for Multiple Pavement Edge with single CSCL segment

• In cases where multiple Pavement Edge segments span a single <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> (median or otherwise), only the BlockfaceID from the Pavement Edge closest to the CSCL segment midpoint was transferred to CSCL.  The other BlockfaceIDs were not conflated to CSCL. An attribute was added to the Pavement Edge database that indicates whether or not each BlockfaceID had been associated with a CSCL segment.<br>

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14506262/e2cfc3f2-018a-11e6-8a19-dd7bf9c57e91.png" /></p>

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14506405/a4614810-018b-11e6-98e7-bacce6f2975e.png" /></p>

[Back to Table of Contents](#table-of-contents)

<br>

#####5. BlockfaceID conflation from Pavement Edge to CSCL - Rule for handling complex intersection/median/bridge scenarios

• In cases of complex intersections with multiple medians and/or elevated roadways/bridges, each level was evaluated individually (i.e., at grade, elevated, etc.) in order to logically determine the appropriate break points on medians and to assign BlockfaceIDs to the correct <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a>. The use of Pavement Edge’s polylineZ information and the use of CSCL’s “level codes” were used to determine which features are on the same vertical plane.<br>
• Only the “straight edges” of medians were assigned to CSCL segments.  Small corner segments for triangular medians were not created.<br>

**The screenshot below shows an example of a “complex” intersection.**

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14506531/42fd8894-018c-11e6-9890-119ed189f684.png" /></p>
<br>
**The screenshot below is the same intersection, but showing only the “at grade” centerlines and Pavement Edgs/Median features. Arrows have been included to depict the assignment of L/R BlockfaceIDs for the “at grade” segments in this intersection.**

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14506559/5ad8b1aa-018c-11e6-9341-85eb1f4fe052.png" /></p>

[Back to Table of Contents](#table-of-contents)

<br>
# PLAZA

**Geometry Type: Polygon**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | Plazas are hard surfaced "parks" adjacent to public sidewalks or pavement edges. |
| **Capture Notes** | All public space plazas were captured or updated.  Where a plaza is connected to a sidewalk by steps, the steps were considered to be part of the plaza polygon. Planters at the edge of plaza were included as part of the plaza boundary.  Plazas are partitioned from medians and / or sidewalks when adjacent to such features. Walkways within the plaza were captured as part of the overall plaza polygon and were not considered a separate polygon. |
| **Features Excluded** | Private plazas were not captured. | 
| **Feature View** | <br><p align="center"><img src="https://cloud.githubusercontent.com/assets/17553952/14298127/215672c8-fb51-11e5-9caf-ea052fbfb3f4.png" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# RAILROAD

**Geometry Type: Polyline**

**Includes the following features:** [Railroad](#subtype-railroad), [Elevated Railroad](#subtype-elevated-railroad), [Embankment Railroad](#subtype-embankment-railroad), [Viaduct Centerline](#subtype-viaduct-centerline), [Depression Railroad](#subtype-depression-railroad), [Railway Fence](#subtype-railway-fence), and [Abandoned Railroad](#subtype-abandoned-railroad)

<br>
### Subtype: RAILROAD

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated railroad centerlines. |
| **Capture Notes** | All visible railroad centerlines were collected/updated.<br><br>Hidden railroad centerlines (in tunnels) were copied from existing data with no elevation value or change. |
| **Features Excluded** | n/a |  
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: ELEVATED RAILROAD

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated elevated railroad centerlines. |
| **Capture Notes** | No elevation value was calculated. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: EMBANKMENT RAILROAD

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated embankment railroad centerlines. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: VIADUCT CENTERLINE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated viaduct railroad centerlines. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a |  
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: DEPRESSION RAILROAD

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated open cut depression railroad centerlines. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a |  
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: RAILWAY FENCE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated open railway fence lines. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a |
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: ABANDONED RAILROAD

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated abandoned railroad centerlines. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Railroad Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **NAME** | Name of Railroad. |<br><br>

[Back to Table of Contents](#table-of-contents)

<br>
# RAILROAD STRUCTURE

**Geometry Type: Polygon**

**Includes the following structures:** [Subway/Train Station](#subtype-subwaytrain-station), [Elevated Subway/Train Station](#subtype-elevated-subwaytrain-station), [Ventilation Grate](#subtype-ventilation-grate), [Emergency Exit](#subtype-emergency-exit), and [Transit Entrance](#subtype-transit-entrance)

<br>
### Subtype: SUBWAY/TRAIN STATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated all stand-alone subway and train stations, and their platforms.<br><br> These structures were found on terrain level or lower. |
| **Capture Notes** | Roof outlines were delineated to include any underlying stairways. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: ELEVATED SUBWAY/TRAIN STATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated all elevated subway and train stations, and their platforms. |
| **Capture Notes** | Roof outlines were delineated to include any underlying stairways. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: VENTILATION GRATE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Ventilation grates were be captured throughout the city. |
| **Capture Notes** | These locations are not dependent on vicinity to subway centerline. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: EMERGENCY EXIT

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated all emergency exits on railroad structures. |
| **Capture Notes** | Usually identified as painted yellow plates/grates for subways. Used ROW of existing subway centerlines as guide. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: TRANSIT ENTRANCE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Updated all transit entrances.  |
| **Capture Notes** | Usually identified as painted stairs for subways.  Used ROW of existing subway centerlines as guide. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Railroad Structure Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **NAME** | Name of Railroad. |<br><br>

[Back to Table of Contents](#table-of-contents)

<br>
# RETAINING WALL

**Geometry Type: Polyline**

**Includes the following features:** [Retaining Wall](#subtype-retaining-wall) and [Railroad Retaining Wall](#subtype-railroad-retaining-wall)

<br>
### Subtype: RETAINING WALL

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Walls that retain earth from falling on transportation features. |
| **Capture Notes** | n/a |
| **Features Excluded** | Walls in backyards used for landscape were not captured.<br><br>Walls in areas under construction
(excavation) were not captured. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: RAILROAD RETAINING WALL

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Walls that retain earth from falling on railroad bed. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# ROADBED

**Geometry Type: Polygon**

**Includes the following features:** [Roadbed](#subtype-roadbed), [Intersection](#subtype-intersection), [Driveway](#subtype-driveway), and [Shoulder](#subtype-shoulder)

<br>
### Subtype: ROADBED

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Roadbed represents the interior polygon of pavement edge. The edges of these features are coincident with the linear feature class [Pavement Edge](#pavement-edge). |
| **Capture Notes** | Converging roadbeds were not split when it crossing one another at different elevations (e.g. on ramps that cross each other). Roadbed was usually cut by [Median](#median) features (e.g., curb & grass) with the exception of painted, barrier and fence medians. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: INTERSECTION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Portion of roadbed where three (3) or more roadways meet up with one another.  Intersections were composed using features compiled and updated in [Pavement Edge](#pavement-edge). |
| **Capture Notes** | Special care was applied at intersections with a slight offset to ensure that such areas were captured and attributed as an intersection.<br><br>The location where two alleys meet is considered an intersection and was captured as intersection roadbed. |
| **Features Excluded** | When two (2) roadways form a “T”, the ending road was closed off so that the continuing roadbed edge forms a straight line (in [Pavement Edge](#pavement-edge)). Not, these "T" locations were not captured as intersection roadbed. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: DRIVEWAY

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | All driveways > 200 feet in length and a minimum width of eight feet.  |
| **Capture Notes** | These driveways may service one or multiple homes and there is no distiction between paved or unpaved surfaces. Driveways were compiled from [Pavement Edge](#pavement-edge).<br><br>Since Driveways have centerlines, if the corresponding <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> has a name, that name is part of the main roadbed feature code. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: SHOULDER

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | All shoulders on the roadway that may be used as a “break-down” area for vehicles or used by emergency vehicles to pass traffic. Shoulders are paved or gravel areas outside of the travel lane (as determined by paint markings) suitable for emergency vehicles to pass. |
| **Capture Notes** | Shoulders were collected along highways (as determined by <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> “RW_TYPE” = 2, 3, or 9 and excluding “SEGMENT_TYPE" = G or F.) only. <br><br>A curb separating an elevated paved surface from the roadway and between the roadway and a barrier median is a shoulder. <br><br>Painted areas are considered shoulders. Should a painted shoulder area be tapered, the entire shoulder was captured as long as the shape was at least 8 feet wide. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# SHORELINE

**Geometry Type: Polyline**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Significant changes (longer than 10 feet) along shorelines were updated to reflect new conditions. |
| **Capture Notes** | When existing shoreline follows the general shape of the shoreline in the imagery, but is offset due to tidal conditions, were not updated.<br><br>Streams greater than 8 feet that intersect bay/ocean were included as part of the shoreline.  When such conditions exist, those features were used and combined with [Hydrography](#hydrography). |
| **Features Excluded** | n/a |
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# SIDEWALK

**Geometry Type: Polygon**

**Includes the following features:** [Row Sidewalk](#subtype-row-sidewalk) and [Interior Sidewalk](#subtype-interior-sidewalk)

<br>
### Subtype: ROW SIDEWALK

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | All paved sidewalks that are located along or adjacent to the ROW (i.e. building to building). |
| **Capture Notes** | In areas of construction, sidewalks were collected along an imaginary line to complete polygon.<br><br>In areas where equipment is stored or installed on sidewalk, the full extent of sidewalk was approximated.<br><br>In areas where protection or scaffolding (pedestrian protection from overhead construction) is placed over sidewalk, sidewalk remained unchanged from existing data (not updated).<br><br>Sidewalks were collected when crossing large medians or traffic islands.<br><br>Sidewalks overlap the exit and entrance portion(s) of parking lot features.<br><br>Sidewalks overlap driveways, but not alleys. Sidewalk will be continued under bridges and overpasses if they are visible on both sides of the structure. |
| **Features Excluded** | Openings in sidewalk (for landscaping and trees) were not captured.<br><br>Large, paved open spaces in front of buildings and outside of the public ROW (may have trees and landscaping) will be included in [Plaza](#plaza) and were not captured as sidewalk. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: INTERIOR SIDEWALK

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | All paved sidewalks for all interior sidewalk that are located interior to the ROW. |
| **Capture Notes** | The business use of this feature is to identify potential areas, outside of the public Right of Way (ROW), that could permit emergency vehicles through travel.<br><br>In areas of construction, sidewalks were collected along an imaginary line to complete polygon.<br><br>In areas where equipment is stored or installed on sidewalk, the full extent of sidewalk was approximated.<br><br>In areas where protection or scaffolding (pedestrian protection from overhead construction) is placed over sidewalk, sidewalk remained unchanged from existing data (not updated). |
| **Features Excluded** | Openings in sidewalk (for landscaping and trees) were not captured. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# SIDEWALK CENTERLINE

**Geometry Type: Polyline**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | These featuers represent interior sidewalk centerlines for all interior sidewalk polygon features (not for the ROW Sidewalk). |
| **Capture Notes** | The business use of this feature is to identify potential areas, outside of the public Right of Way (ROW), that could permit emergency vehicles through travel. Interior Sidewalk Centerlines were extended beyond the Interior Sidewalk Polygons when connecting to a <a href="https://data.ny.gov/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b/about">CSCL</a> feature. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# STREET FURNITURE POINT

**Geometry Type: Point**

**Includes the following features:** [City Benches](#subtype-city-benches), [Mailboxes](#subtype-mailboxes), [Telephone Booths](#subtype-telephone-booths), [Munimeters](#subtype-munimeters), [Ticket Vending Machines](#subtype-ticket-vending-machines), and [Street Seats](#subtype-street-seats)

<br>
### Subtype: CITY BENCHES

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All Benches on sidewalks and within a 10ft buffer from sidewalk. |
| **Capture Notes** | n/a |
| **Features Excluded** | Benches within park boundaries were not captured, unless they are positioned within 10ft of sidewalk. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: MAILBOXES

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All US Postal Mailboxes on sidewalk and within a 10ft buffer from sidewalk. |
| **Capture Notes** | Must represnent feestanding public mail receptacle, typically painted blue. |
| **Features Excluded** | Mailboxes built into a structure were not captured.<br><br>Mailboxes existing under any type of awning or overhead obstruction were not captured. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: TELEPHONE BOOTHS

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All telephone booths on sidewalk and within a 10ft buffer from sidewalk. |
| **Capture Notes** | Single or multiple phone locations were collected, some enclosed and some open. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: MUNIMETERS

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All munimeters on sidewalk and within a 10ft buffer from sidewalk. |
| **Capture Notes** | Features must be free-standing units. |
| **Features Excluded** | Curbside parking meters were not captured. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: TICKET VENDING MACHINES

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All ticket vending machines on sidewalk and within a 10ft buffer from sidewalk. |
| **Capture Notes** | Features must be free-standing units. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: STREET SEATS

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | Any fixed public seating on sidewalk, not included as a bench, were captured as street seats. |
| **Capture Notes** | n/a |
| **Features Excluded** | Street seats within park boundaries were not captured. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# STREET FURNITURE POLY

**Geometry Type: Polygon**

**Includes the following features:** [Bus Shelters](#subtype-bus-shelters), [Newsstands](#subtype-newsstands), [Automatic Pay Toilet](#subtype-automatic-pay-toilet), [Bike Shelters](#subtype-bike-shelters), [Bike Corral](#subtype-bike-corral), [Planters](#subtype-planters), and [Information Kiosks](#subtype-information-kiosks)

<br>
### Subtype: BUS SHELTERS

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All bus shelters on sidewalk and within a 10ft buffer from sidewalk. |
| **Capture Notes** | These features must be semi-enclosed, with a roof structure. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: NEWSSTANDS

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All newsstands on sidewalk and within a 10ft buffer from sidewalk. Free standing, rectangular booth typicaly with an overhanging roof. |
| **Capture Notes** | Only base of structure captured, not the roof overhang (when present). |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: AUTOMATIC PAY TOILET

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All automatic pay toilets on sidewalk and within a 10ft buffer from sidewalk. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BIKE SHELTERS

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All bike shelters on sidewalk and within a 10ft buffer from sidewalk. |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: BIKE CORRAL

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All bike corrals on sidewalks and within a 10ft buffer from sidewalk. |
| **Capture Notes** | n/a |
| **Features Excluded** | Stands for bicycles were not captured.  | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: PLANTERS

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All planters where all of its sides are 3’ or greater. |
| **Capture Notes** | Planters were captured only if on sidewalks and within a 10ft buffer from sidewalk. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: INFORMATION KIOSKS

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | All information kiosks on sidewalk and within a 10ft buffer from sidewalk.<br><br>Rectangular, free-standing booths at that are at least 10 square feet. |
| **Capture Notes** | n/a |
| **Features Excluded** | Freestanding information boards or signs were not captured. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# SWIMMING POOL

**Geometry Type: Polygon**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery. |
| **Features Captured** | All in-ground swimming pools, regardless of shape, on the inside (water) of the pool. |
| **Capture Notes** | n/a |
| **Features Excluded** | Round, above-ground swimming pools were not captured, nor pools that are on buildings.<br><br>Fish ponds and landscape ponds of irregular shape, and low-sided kiddie pools, were not collected.  | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
# TRANSPORT STRUCTURE

**Geometry Type: Polygon**

**Includes the following features:** [Bridge](#subtype-bridge), [Tunnel](#subtype-tunnel), [Rail Bridge](#subtype-rail-bridge), [Pedestrian/Bike Bridge](#subtype-pedestrianbike-bridge), [Railroad Viaduct](#subtype-railroad-viaduct), and [Overpass](#subtype-overpass)

<br>
### Subtype: BRIDGE

|     |     |
| --- | --- |
| **Source Databases** | Newly collected from 2014 imagery. |
| **Features Captured** | Structures erected over obstacles for road traffic (road, railroad, hydrography). Bridge deck outlined from joint to joint when on-and off-ramp(s) are on ground.  Large bridges with on-ramps and off-ramps were collected from point elevation begins (bridge elevation subype. |
| **Capture Notes** | Features can overlap so that bridge is not split where it crosses another bridge feature. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: TUNNEL

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Used tunnel portal to digitize. |
| **Capture Notes** | Maintained delineation from existing data when available. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: RAIL BRIDGE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Structure erected over obstacle for railroad traffic (road, railroad, hydrography). |
| **Capture Notes** | n/a |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: PEDESTRIAN/BIKE BRIDGE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Strutures allowing pedestrians/bicycles to cross transportation features.  |
| **Capture Notes** | Where applicable, outline includes stairs.  Can connect between buildings (snapped to building footprint). |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: RAILROAD VIADUCT

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Bridge composed of several small arches, mostly over water. |
| **Capture Notes** | Visible changeover from solid ground to viaduct is outlined. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
### Subtype: OVERPASS

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | Structure erected over road, whereas the lower road has been excavated and has retaining walls on the side. |
| **Capture Notes** | Overpass is at terrain level. |
| **Features Excluded** | n/a | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)

<br>
#### Transport Structure Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **NAME** | Name of Transportation Structure. |<br><br>

[Back to Table of Contents](#table-of-contents)

<br>
# UNDER CONSTRUCTION UNKNOWN

**Geometry Type: Polygon**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics. |
| **Features Captured** | All areas under construction (excavation) or deposits of material (storage) at their outer boundary. |
| **Capture Notes** | Entrance to construction site was ignored and not snapped to sidewalk nor pavement edge. |
| **Features Excluded** | Building foundations or partially demolished buildings were not collected.<br><br>Individual excavation or deposit areas were not partitioned. | 
| **Feature View** | <br><p align="center"><img src="" /></p> |
| **Photo** | <br><p align="center"><img src="" /></p> |<br><br>
[Back to Table of Contents](#table-of-contents)
