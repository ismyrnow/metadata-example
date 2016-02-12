#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CSCL_STREET_CENTERLINE&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polyline*
######Source Databases: Update from imagery, existing planimetrics

######Description:

CSCL geometry will not be edited; edits made to CSCL (Centerline) will be limited to attributes. 

As a general rule, no attributes will be assigned to the “generic” or “faux” CSCL centerline segments.
SEGMENT_TYPE NOT IN (‘F’, ‘G’)

All other types of segments will get attributes when they have corresponding PavementEdge/Roadbed features. In some cases this will include adding attributes to driveways, alleys, etc.

If no roadbed exists, these attributes will not be captured.
