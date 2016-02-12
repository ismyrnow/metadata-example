#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CEMETERY OUTLINE&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Update cemetery boundary from new imagery.

Do NOT collect individual headstones, graves, or interior boundaries.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RECREATIONAL AREA&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Outline recreational - exclusive (outside) of NYC designated parks; may be used for picnic or other recreational use. These include areas such as Brooklyn Bridge Park and the High Line. Recreational areas must contain at least one of the following:

a) Benches,
b) Swings
c) Play area

Hardscape recreation areas will be collected differently than softscape recreational areas.

Hardscape recreational areas have either hard surfaces or sand. These areas will be captured as discrete polygons following the edges of these areas precisely.

Softscape recreational areas are grassy areas for football/baseball/other. These areas will be captured as a single polygon (ie not discrete polygons) and snapped to other features (e.g. sidewalks, roadbed, hydro, etc.) where applicable.

When hardscapes and softscapes exists adjacent to one another, the entire area will be captured by a single polygon.

Medians with features in the preceeding list will be captured as a median and not a recreational area.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;VACANT AREA&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing data Digital Tax Map (DTM)

######Description:

This is intended to be a vacant lot where a building could potentially be built and is associated with a tax lot polygon.

Outline vacant areas on map. Vacant defined as containing no structures.  Use the DTM and currently captured planimetrics (BUILDING_FOOTPRINT) to determine the location of the vacant areas.  Collect the actual shape using physical features that typically form the boundary of a property such as fences, hedgerow, etc.
Vacant Area will extend to sidewalk or roadbed edge.
