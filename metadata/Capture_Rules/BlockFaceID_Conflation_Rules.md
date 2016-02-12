*This section includes the following capture rules pertaining to BlockfaceID conflation from PavementEdge to CSCL for these special/complex cases:*<br>
####1. Capture Rule for missing CSCL
**BlockfaceID conflation from PavementEdge to CSCL - Rule for missing CSCL:**

•	If no CSCL feature exists on an existing roadbed with PavementEdge, the production team will break the PavementEdge based as needed on the visual center of where a CSCL Centerline might go and then assign L/R BlockfaceIDs to the PavementEdge.  However, these BlockfaceIDs will not be conflated to any CSCL segments (and these PavementEdge features will be flagged as having a BlockfaceID that was not conflated to CSCL). 

####2. Capture Rule for Medians
**2. BlockfaceID conflation from PavementEdge to CSCL - Rules for Medians:**

•	When a CSCL segment is bounded on one or both sides by a median, the longest edges of median PavementEdge will be assigned BlockfaceIDs, which will be conflated onto applicable adjacent CSCL segments.

•	Assign BlockfaceIDs to PavementEdge for all medians except painted medians.

•	Conflate to CSCL where no PavementEdge derived BlockfaceID takes priority, and there is a CSCL segment that corresponds to the long edge of the median.

•	In cases where medians are within medians the conflating median is the majority (containing) median.

•	PavementEdge features on a median will be flagged as having a BlockfaceID that was not conflated to CSCL .

####3. Capture Rule for Multiple CSCL with Single PavementEdge
**BlockfaceID conflation from PavementEdge to CSCL -  Rule for Multiple CSCL Segments with a Single PavementEdge**

•	In cases where there are multiple CSCL segments running along a single PavementEdge (median or otherwise), the BlockfaceID from the PavementEdge will be conflated to the CSCL segments that correspond to the single PavementEdge.

####4. Capture Rule for Multiple PavementEdge with single CSCL segment
**BlockfaceID conflation from PavementEdge to CSCL - Rule for Multiple PavementEdge with single CSCL segment**

•	In cases where multiple PavementEdge segments span a single CSCL (median or otherwise), only the BlockfaceID from the PavementEdge closest to the CSCL segment midpoint will be transferred to CSCL.  The other BlockfaceIDs will not be conflated to CSCL. An attribute will be added to the PavementEdge database that indicates whether or not each BlockfaceID had been associated with a CSCL segment.

####5. Capture Rule for handling complex intersection/median/bridge scenarios
**BlockfaceID conflation from PavementEdge to CSCL - Rule for handling complex intersection/median/bridge scenarios**

•	In cases of complex intersections with multiple medians and/or elevated roadways/bridges, AppGeo will evaluate each “level” individually (i.e., at grade, elevated, etc.) in order to logically determine the appropriate break points on medians and to assign BlockfaceIDs to the correct CSCL. The use of PavementEdge’s polylineZ and the use of CSCL’s “level codes” will be used to determine which features are on the same vertical plane. 

•	Only the “straight edges” of medians will be assigned to CSCL segments.  Small corner segments for triangular medians will not be created.
