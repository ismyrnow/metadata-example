#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PARK BOUNDARY&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

All Park features will be determined by the source database:  DPR_Parks.gdb

Park boundaries will be determined by the DPR_REP_PROPERTY feature class. Do not delineate interior road systems within parks. Capture the outside perimeter of the park.

The park boundary will cover the entire park as a single polygon, regardless of special features such as baseball diamonds or tennis courts.  

Do NOT “cut-out” the special features from the park boundary.

Park names (SIGNNAME and source column) and park numbers (GISPROPNUM source column) are to be transferred from source databases to park boundaries and special features.

The delineation of the outer edge of each park boundary will be coincident with the “intended” boundary feature as determined by the Parks Department. Intended boundary feature will be curbs, green areas, sidewalks, etc. and will vary from park to park.  At times, the intended boundary feature will vary within the same park.

In general, if the source data has a single boundary polygon extending across other planimetric features (e.g. roads), the planimetric park boundary will follow the source data.

On a rare occasion, there may be no apparent physical boundary feature to delineate the Park boundary.  On these occasions, copy the feature “as is” from the source database.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BASEBALL/SOFTBALL FIELD&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline sandy area (diamond) in softball/baseball fields – can have different size and can be also painted on hard surface.

Extend the polygon to the backstop of the field and include 1st and 3rd base coaching boxes.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BASKETBALL COURT&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline boundary of individual court – can be full-court or half-court.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HANDBALL&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Collect handball court (hard surface with wall). If multiple courts, compile outside and place division line between individual
courts.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MULTIPURPOSE COURT&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline multipurpose field – mostly hard surface with different markings for different activities.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TENNIS COURT&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Collect tennis court (hard surface) –for multiple courts, delineate along outer painted line (baseline and sideline) and place division line between individual courts. 

Within NYC Parks Do NOT collect individual courts. 

Do NOT collect private tennis courts (on roofs or hotels, etc.).  

Do not extend the polygon to the fence surrounding the tennis court area.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;VOLLEYBALL&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline volleyball court (look for distinct markings on hard surface).

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;FOOTBALL FIELD&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline football field.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;SOCCER FIELD&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline soccer field – grassy surface when outline is present.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;GOLF COURSE&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline golf course along fence or other man-made boundary.

Do NOT outline greens, tees, fairways, sand traps, shelters, or cart paths.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;POOLS&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline public pool areas.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;TRACK&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline track around grassy area.

Do NOT collect when painted on concrete surface.

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;SKATING RINK&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Outline skating/hockey rink (look for distinct markings on hard surface).

<br>

#####Feature Code | *type*:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;GREENSTREETS&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;*polygon*

######Source Databases: Update from imagery, existing planimetrics, Parks database

######Description:

Using the DRP_REP_Greenstreet feature class as the definitive source, these areas will be updated and attributed
using the source data. Name will be populated from the SITENAME source column and park numbers will be populated from the GISPROPNUM source column.

All the rules for defining park boundaries will apply for defining Greenstreets.
