#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ROADBED&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Interior polygon of pavement edge. This feature should be coincident with PAVEMENT_EDGE polyline feature.

Do not split the roadbed when it crosses another roadbed at different elevations (e.g. on ramps that cross each other).

Roadbed should be cut by MEDIAN features (curb & grass) with the exception of painted, barrier and fence medians.

Special care should be applied to ensure that the shoulder on highways is not confused as a sidewalk.

<br></br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;INTERSECTION&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Interior polygon over road intersections using features compiled and updated in the Pavement edge layer. Generation of small (city block) polygons with separate polygons at intersections. Placement of intersection lines using centerline nodes for automatic and manual placement. Intersection polygon will be created by establishing the shortest distance from the intersection node to PAVEMENTEDGE Feature.

Special care should be applied at intersections with a slight offset to ensure these features are captured and attributed as an intersection.

Intersections forming a “T” or any other intersection of two roads where one road is continuing and one road is ending, the ending road will be closed off so that the continuing roadbed edge forms a straight line.

The location where two alleys meet is considered an intersection and will be an intersection roadbed.

<br></br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;DRIVEWAY&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Collect all driveways > 200 feet in length, may service one or multiple homes. Do not distinct between paved or unpaved.
Compile driveway from the PAVEMENTEDGE feature.

Driveways allow access from a road to one or multiple buildings. Check with parcel database – has to be on a parcel or over adjacent parcels.  Must be longer than 200 feet, regardless of surface condition. Do not confuse with alley. Will have a minimum width of eight feet.  Driveways DO have centerlines.  If a driveway has a name in the CSCL then it should be part of the main roadbed feature code.

<br></br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;SHOULDER&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery

######Description:

Collect all shoulders on the roadway that may be used as a “break-down” area for vehicles or used by emergency vehicles to pass traffic.  Shoulders are paved or gravel areas outside of the travel lane (as determined by paint markings) suitable for emergency vehicles to pass. Shoulders will be collected along highways (as determined by CSCL “RW_TYPE” = 2, 3, or 9 and excluding “SEGMENT_TYPE" = G or F.) only. Shoulders will only be collected when the width is suitable for vehicle travel (8 feet minimum).

A curb separating an elevated paved surface from the roadway and between the roadway and a barrier median is a shoulder. Painted areas are considered shoulders as illustrated in the following graphics.

Should a painted shoulder area be tapered, the entire shoulder will be captured as long as the shape is at least 8 feet wide.
