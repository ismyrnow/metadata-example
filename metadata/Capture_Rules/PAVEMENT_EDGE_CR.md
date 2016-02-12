#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EDGE OF PAVEMENT&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polylineZ*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Update all segments between pavement and other surfaces or features (i.e. Curbs, sidewalks, or grass.)

Each segment shall be continuous across a blockface (typically from one intersection to the next – along that side of the road). The vertex between two segments should be located at the street corner. EOP features will be continuous across driveways, alleys, or access to parking. The one exception to this rule is where a street segment changes names (as determined by CSCL Centerline names) outside of any street intersections. In these cases, the existing CSCL break (node) will be used to create corresponding breaks in PAVEMENTEDGE segments.  

For cul-de-sacs, two segments will be created. The CSCL centerline will be used to define the breakpoints of the PAVEMENTEDGE segments.

Dead end streets will terminate where the tax map crosses the road.  Two segments will be created on left and right sides of CSCL

On highways, PavementEdge will correspond to the ‘roadbed’ sub-feature class in roadbed, and do not include the shoulder.

See [**BlockfaceID Conflation Rules**](BlockFaceID_Conflation_Rules.md)

<br></br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AIRPORT RUNWAY&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polylineZ*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Collect outer-edge of all paved features, including runways, taxiways and aprons. 

Share edge with building feature. Collect airport features up to surrounding fence or gates.

<br></br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ALLEY&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polylineZ*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Alley is defined as a narrow unnamed street that allows access to buildings/garages other than from the road. Normally allows
access to the interior of a block or to the back of a house. Snap to roadedge.

Some narrow streets with CSCL names were previously captured as alleys or hidden alleys. The designation was also used for
named step streets and possibly for some hidden park paths and bike paths.

Use the CSCL value of: RW_TYPE=10 to determine the alley pavementedge.  Note that the CSCL is only a reference – there may be alleys that are not have this field attribute.
