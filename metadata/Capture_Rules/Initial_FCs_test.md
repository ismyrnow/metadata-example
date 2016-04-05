**Table of contents**<br>
&nbsp;&nbsp;&nbsp;&nbsp;[General Attribute Information](#general-attribute-information)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Boardwalk](#boardwalk)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Building Footprints](#building-footprints)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: BUILDING](#subtype-building)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: GARAGE](#subtype-garage)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: BUILDING U/C (Building Under Construction](#subtype-building-uc-building-under-construction)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: SKYBRIDGE](#subtype-skybridge)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Building Footprint Attributes](#building-footprint-attributes)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Building Footprint Diagrams](#building-footprint-diagrams)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Curb](#curb)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Elevation](#elevation)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: BUILDING ELEVATION](#subtype-building-elevation)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: WATER ELEVATION](#subtype-water-elevation)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: SPOT ELEVATION](#subtype-spot-elevation)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtype: BRIDGE ELEVATION](#subtype-bridge-elevation)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Elevation Attributes](#elevation-attributes)<br>
&nbsp;&nbsp;&nbsp;&nbsp;[Plaza](#plaza)<br>

# General Attribute Information

The following attribute information applies to all feature classes.  Additional attributes specific to a given feature class are listed within the details for that feature class.

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">**Description**</p> |
| **Source_ID** | Unique feature Identification Number |
| **Feature_Code** | Indicates the type of feature  |
| **Sub_Feature_Code** | (where applicable) indicates a subset of features within a given “Feature_Code” set  |
| **Status** | Field indicating the feature status as it fits into one of the following categories:<br>a) NEW. A feature captured for the first time during the 2014 planimetrics update project.<br>b) UPDATED. The feature existed previously but has been updated during the 2014 planimetrics update project.<br>c) UNCHANGED. The feature is unchanged from the source planimetrics database. |

<br>
# Boardwalk

**Type: Polygon**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery |
| **Features Captured** | Boardwalks along beachfront|
| **Capture Notes** | Maintain beach outline/shoreline |
| **Features Excluded** | n/a | 
| Map |  |
| Photo |  |

<br>
# Building Footprints

**Type: Polygon**

**Includes the following structures:** [Building](#subtype-building), [Garage](#subtype-garage), [Under Construction Unknown](#subtype-building-uc-building-under-construction), and [Skybridge](#subtype-skybridge)


### Subtype: BUILDING

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery<br><br>Used existing building database for reference and for BIN values. |
| **Features Captured** | Collected all buildings with well-defined walls and roofs that are >400 sq. feet and taller than 12 feet.<br><br>Buildings with <12 feet height but with BIN were captured.<br><br>Buildings with BIN but <400 sq. feet were captured.<br><br>Buildings with flat roofs were captured on roof outline, capturing the largest outline (excluding overhangs, awnings, construction features, etc.).<br><br>Buildings with pitched roofs were captured on the building footprint.<br><br>Carports, when attached to main building, were included in the outline. Do not collect interior divisions within buildings were not captured (used existing building layer and BIN as guide). |
| **Capture Notes** | Use parcel data and BIN as guidance for collection. Where the parcel data indicates that a building should be two or more geometries AND there is NO physical indication, split the building using the parcel lines. Where the parcel data indicates that a building should be two or more geometries AND there is a physical indication, split the building using the physical indications. If an existing building is going to split into several new buildings, keep the original BIN in only one of the new buildings (ideally the largest) and assign a million BIN to the rest. Do not duplicate BINS.<br><br>Building footprints that are adjacent, have different BINS and are on one tax lot should be flagged and verified during update.<br><br>If a building is demolished (i.e., if the building has a different shape), the BIN is also deleted and is not to be used for any new building geometry.<br><br>Small triangles denote a permit is out to construct a new building at the location and are added by DoITT building editors. These triangles should be removed when new buildings are added. Therefore if a new building has been constructed in the new orthos please collect building, transfer attributes from triangle to building, and delete triangle. If no new building is visible on the orthos, please leave triangles alone (and they will be exceptions in the QC model). |
| **Features Excluded** | The following features are not captured:<br>•  temporary trailers, tents, or roofs at gas stations (over pumps).<br>• roofs (overhang) to gas stations, unless connected to building.<br>• movable jet bridge for access to aircraft<br>• awnings, scaffolds, or sidewalk sheds. | 
| Map |  |
| Photo |  |

<br>
### Subtype: GARAGE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery<br><br>Used existing building database for reference and for BIN values.<br><br>Used DOF TaxMapas a reference |
| **Features Captured** | CAll garages were captured, regardless of size.  To be considered a garage, the structure must have a driveway (paved or unpaved) for road  access, and be able to store one or more cars. |
| **Capture Notes** | Special care should be applied to ensure sheds are not confused with garages. In general, standard dimensions for detached garages are approximately 12’x20’ or 14’x20’<br><br>Use Parcel layer to place garages within parcel or at parcel boundary – check for special cases where parcel boundary clearly crosses garage. In these cases, either split the garage using physical features, or use the property line where there is no distinguishing physical feature.<br><br>In cases where there is no BIN for the garage, a “dummy” BIN will be assigned as follows:<br>• 1000000 for Manhattan,<br>• 2000000 for Bronx,<br>• 3000000 for Brooklyn,<br>• 4000000 for Queens,<br>• 5000000 for Staten Island |
| **Features Excluded** | Small tool or storage sheds in backyards which have no visible car access were not captured | 
| Map |  |
| Photo |  |

<br>
### Subtype: BUILDING U/C *(Building under Construction)*

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery<br><br>The existing DoITT building database was used for reference and for BIN values. |
| **Features Captured** | Buildings that are under construction and have outside walls that clearly indicate the shape of the building were captured. |
| **Capture Notes** |  |
| **Features Excluded** | Buildings were not captured when only the foundation was visible or building was being destroyed. | 
| Map |  |
| Photo |  |

<br>
### Subtype: SKYBRIDGE

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery |
| **Features Captured** | Elevated walkways that connect buildings were captured as separate building polygons and coded as “Skybridge”. |
| **Capture Notes** | Skybridges will be populated with the “HEIGHT_ROOF” attribute only (not Ground Elevation).<br><br>These were assigned a “dummy” million BIN during capture. |
| **Features Excluded** |  | 
| Map |  |
| Photo |  |

<br>
#### Building Footprint Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">Description</p> |
| **HEIGHT_ROOF** | Building roof height is calculated as the difference between ground elevation of the building and the roof elevation value.  The roof elevation is the highest point of the roof itself (see BUILDING ELEVATION in the ELEVATION Feature Class). See diagrams below. |
| **GROUND_ELEVATION** | Lowest Elevation at the building ground level.  Calculated from LiDAR or photogrammetrically. |

<br>
#### Building Footprint Diagrams
#####<p align="center">**Calculating HEIGHT_ROOF**</p>

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14287639/6f62b2fe-fb21-11e5-9515-35784cf3d534.png" /></p>

<p align="center"><img src="https://cloud.githubusercontent.com/assets/3277588/14287724/e7b77b72-fb21-11e5-8b08-4a83218c3b0e.png" /></p>

<br>
# Curb

**Type: Polyline**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery |
| **Features Captured** | All curbs between roadbed pavement and other surfaces (i.e., within the street right-of-way) were captured. |
| **Capture Notes** |  |
| **Features Excluded** | Curbs inside Parking lots will not be captured. | 
| Map |  |
| Photo |  |

<br>
# Elevation

**Type: Point**

**Includes the following structures:** [Building Elevation](#subtype-building-elevation), [Water Elevation](#subtype-water-elevation), [Spot Elevation](#subtype-spot-elevation), and [Bridge Elevation](#subtype-bridge-elevation)


<br>
### Subtype: BUILDING ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics |
| **Features Captured** | Elevation points were captured for all building footprint features. |
| **Capture Notes** | Elevation of the highest portion of the roof of a building, excluding antennas and roof fixtures such as air conditioning (AC), elevator shafts, chimneys, etc.<br><br>Elevation value will be transferred to building outline to calculate the building height attribute. |
| **Features Excluded** |  | 
| Map |  |
| Photo |  |

<br>
### Subtype: WATER ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics |
| **Features Captured** | Elevation points were captured on standing water (ponds, reservoirs, lakes). |
| **Capture Notes** |  |
| **Features Excluded** |  | 
| Map |  |
| Photo |  |

<br>
### Subtype: SPOT ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics |
| **Features Captured** | Spot elevations were captured on paved, unpaved, and alley subtypes in CSCL Centerline and all Interior Sidewalk Centerline.   Elevation points were placed in the center of the roadbed (coincident with CSCL), captured at beginning, mid-point, end, and at 200’ spacing of the visible roadbed. |
| **Capture Notes** | In areas where the PAVEMENTEDGE has been updated, any existing SPOT elevations will be updated.<br><br>For new streets, new spot elevations were created in the center of the roadbed according to the following rules:<br>1) Placed at Intersections (might not necessarily be at the same location as the node from the CL, one point per intersection even on complex intersections).<br>2) Placed Every 200 feet when midpoint of bridge or city block exceeds distance.<br>3) Placed on paved, unpaved, alley subtypes in CSCL Centerline and all of Interior Sidewalk Centerline.  Spot elevation will not be added to a CSCL if no roadbed exists (e,g, area is under construction).<br>4) Mid-Street segment – at the approximate mid-point of a street segment. |
| **Features Excluded** | Spot elevations were not be captured on a CSCL if no roadbed exists | 
| Map |  |
| Photo |  |

<br>
### Subtype: BRIDGE ELEVATION

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery and existing planimetrics |
| **Features Captured** |  |
| **Capture Notes** | This is a subset of spot elevations. Elevation points were captured at the beginning, mid-point, end, and at 200’ spacing of the visible deck of bridges and overpasses. |
| **Features Excluded** | Elevation points were not collected for pedestrian/bike bridges. | 
| Map |  |
| Photo |  |


<br>
#### Elevation Attributes

|     |     |
| --- | --- |
| <p align="center">**Attribute**</p> | <p align="center">Description</p> |
| **Elevation** | Field measuring surface elevation above sea level (in feet) |

<br>
# Plaza

**Type: Polygon**

|     |     |
| --- | --- |
| **Source Databases** | Updated from 2014 imagery |
| **Features Captured** | Plazas are hard surfaced "parks" adjacent to public sidewalks or pavement edges. |
| **Capture Notes** | All public space plazas were captured or updated.  Where a plaza is connected to a sidewalk by steps, the steps were considered to be part of the plaza polygon. Planters at the edge of plaza were included as part of the plaza boundary.  Plazas cannot overlap medians or sidewalks. Walkways within the plaza were captured as part of the overall plaza polygon and were not considered a separate polygon. |
| **Features Excluded** | Private plazas were not captured. | 
| Map |  |
| Photo |  |
