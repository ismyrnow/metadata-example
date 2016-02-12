**RULE:** *Street CL cannot intersect median of same road except in rare occasions (e.g. at street intersections with medians). Median type hierarchy will be barrier, rail, fence, curb, grass and painted.*<br><br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MEDIAN&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

All medians that physically divide a roadbed are collected and include medians, traffic islands, and Jersey barriers as well as
painted to separate the traffic flow. Medians can be paved and are normally elevated (have a curb) or have dirt or grass.

Medians can have sidewalks crossing them. In this instance, compile outline of largest area.

Do NOT collect barriers in front of buildings.

Do NOT collect jersey barriers to regulate traffic in construction areas or to block-off road access.

The NYC online Bike Lane data will be used a reference to identify potential new medians. Areas where the column ALLCLASSES is equal to I and "I,II" are likely areas to contain new medians. New Medians will exist throughout the City regardless of these bike lane classifications. Thus, this is to be considered a supplemental source only.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MEDIAN_PAINTED&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Medians that have white paved marking (fishbone or striped) shall be collected as Median-painted.  Double yellow lines in the middle of a road are NOT medians. Single independent white medians hatched used to direct traffic are NOT medians- refer to Centerline file.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MEDIAN_CURB&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Median with curb edge regardless of interior content (grass, pavement, concrete, etc.).

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MEDIAN_RAIL&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Median with guardrail outline the curb of the median; For guardrail only- use a fixed width of three (3) feet centered on the fence.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MEDIAN_FENCE&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Median with fence.  If Jersey Barrier has fence collect as Jersey barrier (see hierarchy below).

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MEDIAN_GRASS&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Median with grass/vegetation inside and no curb.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MEDIAN_BARRIER&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Jersey barriers must be of “permanent nature,” i.e., in place to regulate the traffic, and must be displayed with a constant width
of three (3) feet centered on the barrier. Omit those which are moved on a daily basis, like at Manhattan entrances to Lincoln
Tunnel.

In the case where two jersey barriers are placed next to or in short distance of each other, outline the outer-most edge. Do NOT compile as two Jersey barriers.

