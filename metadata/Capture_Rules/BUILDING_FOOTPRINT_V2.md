Table of contents
- [Building Footprints](#building-footprints)
- [Plaza](#plaza)

## Building Footprints

**Includes the following structures:** [Buildings](#subtype-building), [Garages](#subtype-garage), [Under Construction Unknown](#subtype-building-uc-building-under-construction), and [Skybridge](subtype-skybridge)

### Subtype: BUILDING

|     |     |
| --- | --- |
| **Source Databases** | Update from imagery, existing database with BIN |
| **Features Captured** | Collect all buildings with well-defined walls and roofs that are >400 sq. feet and taller than 12 feet.<br><br>Buildings with <12 feet height but with BIN should be captured.<br><br>Buildings with BIN but <400 sq. feet will be captured.<br><br>Buildings with flat roofs will be captured on roof outline, capturing the largest outline (excluding overhangs, awnings, construction features, etc.).<br><br>Buildings with pitched roofs will be captured on the building footprint.<br><br>Carports, when attached to main building, will be included in the outline. Do not collect interior divisions (use existing building layer and BIN as guide). |
| **Capture Process** | Use parcel data and BIN as guidance for collection. Where the parcel data indicates that a building should be two or more geometries AND there is NO physical indication, split the building using the parcel lines. Where the parcel data indicates that a building should be two or more geometries AND there is a physical indication, split the building using the physical indications. If an existing building is going to split into several new buildings, keep the original BIN in only one of the new buildings (ideally the largest) and assign a million BIN to the rest. Do not duplicate BINS.<br><br>Building footprints that are adjacent, have different BINS and are on one tax lot should be flagged and verified during update.<br><br>If a building is demolished (i.e., if the building has a different shape), the BIN is also deleted and is not to be used for any new building geometry.<br><br>Small triangles denote a permit is out to construct a new building at the location and are added by DoITT building editors. These triangles should be removed when new buildings are added. Therefore if a new building has been constructed in the new orthos please collect building, transfer attributes from triangle to building, and delete triangle. If no new building is visible on the orthos, please leave triangles alone (and they will be exceptions in the QC model). |
| **Features Excluded** | Do NOT collect temporary trailers, tents, or roofs at gas stations (over pumps).<br><br>Do NOT collect roofs (overhang) to gas stations, unless connected to building.<br><br>Do NOT collect movable jet bridge for access to aircraft<br><br>Do NOT collect awnings, scaffolds, or sidewalk sheds. | 
| Map | ![Map](http://otile1.mqcdn.com/tiles/1.0.0/map/17/38599/49257.png) |
| Photo | ![Photo](https://pbs.twimg.com/profile_images/595637146054168577/OZ127kGE_400x400.jpg) |

### Subtype: GARAGE

|     |     |
| --- | --- |
| **Source Databases** | Update from imagery, existing database with BIN, DOF TaxMap |
| **Features Captured** | Collect all garages, regardless of size, that can be identified as such, have driveways (paved or unpaved) for road  access, and that store one or more cars. |
| **Capture Process** | Special care should be applied to ensure sheds are not to be confused with garages. Oftentimes, driveways do lead to sheds, so not all structures at a terminating driveway are considered to be garages. Sheds are not to be captured.<br><br>In general, standard dimensions for detached garages are approximately 12’x20’ or 14’x20’<br><br>Use Parcel layer to place garages within parcel or at parcel boundary – check for special cases where parcel boundary clearly crosses garage. In these cases, either split the garage using physical features, or use the property line where there is no distinguishing physical feature.<br><br>In cases where there is no BIN for the garage, a “dummy” BIN will be assigned as follows:<br>• 1000000 for Manhattan,<br>• 2000000 for Bronx,<br>• 3000000 for Brooklyn,<br>• 4000000 for Queens,<br>• 5000000 for Staten Island |
| **Features Excluded** | Do NOT collect when only the foundation is visible or building is being destroyed. | 
| Map | ![Map](http://otile1.mqcdn.com/tiles/1.0.0/map/17/38599/49257.png) |
| Photo | ![Photo](https://pbs.twimg.com/profile_images/595637146054168577/OZ127kGE_400x400.jpg) |

### Subtype: BUILDING U/C *(Building under Construction)*

|     |     |
| --- | --- |
| **Source Databases** | Update from imagery, existing database with BIN |
| **Features Captured** | Capture buildings that are under construction AND their outside walls clearly indicate the shpe of the building. |
| **Capture Process** |  |
| **Features Excluded** | Do NOT collect small tool or storage sheds in backyards which have no visible car access. | 
| Map | ![Map](http://otile1.mqcdn.com/tiles/1.0.0/map/17/38599/49257.png) |
| Photo | ![Photo](https://pbs.twimg.com/profile_images/595637146054168577/OZ127kGE_400x400.jpg) |

### Subtype: SKYBRIDGE

|     |     |
| --- | --- |
| **Source Databases** | Update from imagery |
| **Features Captured** | Capture buildings that are under construction AND their outside walls clearly indicate the shpe of the building. |
| **Capture Process** |  |
| **Features Excluded** | Do NOT collect small tool or storage sheds in backyards which have no visible car access. | 
| Map | ![Map](http://otile1.mqcdn.com/tiles/1.0.0/map/17/38599/49257.png) |
| Photo | ![Photo](https://pbs.twimg.com/profile_images/595637146054168577/OZ127kGE_400x400.jpg) |

## Plaza

|     |     |
| --- | --- |
| **Source Databases** | Update from imagery |
| **Features Captured** | Elevated walkways that connect buildings will be captured as separate building polygons and coded as “Skybridge”. |
| **Capture Process** | Skybridges will be populated with the “HEIGHT_ROOF” attribute only (not Ground Elevation).<br><br>These will be assigned a “dummy” million BIN during capture. |
| **Features Excluded** |  | 
| Map | ![Map](http://otile1.mqcdn.com/tiles/1.0.0/map/17/38599/49257.png) |
| Photo | ![Photo](https://pbs.twimg.com/profile_images/595637146054168577/OZ127kGE_400x400.jpg) |
