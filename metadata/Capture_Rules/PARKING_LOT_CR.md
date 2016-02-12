**NOTE:** Sidewalk outline will cross over parking lot outline only at the entrance and exit.<br><br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PARKINGLOT&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics

######Description:

Collect all parking lots (paved or unpaved) greater than 2,000 sq. feet.

Do NOT collect traffic islands within parking lot.

If building > 400 sq. feet is present, outline building.

Connect to road-edge (curb or edge of pavement) only at entrances and exits.

Do not collect gas stations, private lots, storage areas, etc as parking lots.

Parking areas adjacent to the travel-way BUT NOT separated from the travel-way by a curb or other obstruction are not parking lots. These parking areas are to be part of the roadbed and the pavement_edge should extend to their outside edge of the parking area.  This seems to be the case in the parking area to the west in the example below.

Parking areas adjacent to the travel-way AND separated from the travel-way by a curb or other obstruction are parking lots. The roadbed and pavement_edge are to end or wrap around the parking lot. The parking lot is not to be part of the roadbed. This seems to be the case for the parking area (parking lot) to the east in the example below. This should be captured as a parking lot.
