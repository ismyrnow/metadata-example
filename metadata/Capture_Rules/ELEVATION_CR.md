**NOTE:** *Make sure that vertical accuracy specifications in request for services (RFQ) are met (ASPRS 1”=100’ Class 2).*
<br><br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BUILDING ELEVATION&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*point*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Collect point on the highest portion of the roof of a building, excluding antennas, and roof fixtures such as air conditioning (AC), elevator shafts, chimneys, etc. 

Elevation value will be transferred to building outline to calculate the building height as attribute.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;WATER ELEVATION&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*point*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Collect water elevation on standing water (ponds, reservoirs, lakes).

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;SPOT ELEVATION&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*point*

######Source Databases: Update from imagery, existing planimetrics

######Description:

For the most part, existing spot elevations will not be moved. If existing SPOT elevations are more than 5’ off the existing CSCL Centerline an attribute flag will denote (schema/values are TBD). 

In areas where the PAVEMENTEDGE has been updated, any existing SPOT elevations will be updated.
 
For new streets, new spot elevations will be created in the center of the roadbed according to the following rules:

1) Intersections (might not necessarily be at the same location as the node from the CL, one point per intersection even on complex intersections).

2) Every 200 feet when midpoint of bridge or city block exceeds distance.  DoITT to provide additional spot locations along bridges for verification.

3) Will be captured on paved, unpaved, alley subtypes in CSCL Centerline and all of Interior Sidewalk Centerline.  Spot elevation will not be added to a CSCL if no roadbed exists (e,g, area is under construction).

4) Mid-Street segment – at the approximate mid-point of a street segment.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BRIDGE ELEVATION&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*point*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Bridges/overpass – beginning, mid-point end, and at 200’ spacing of the visible bridge deck. Subset of Spot Elevations.

Do NOT collect on pedestrian/bike bridges.

