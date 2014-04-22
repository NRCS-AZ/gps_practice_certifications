#Practice Certifications#
##Trimble GPS Field Collection with CartoPac##


###PURPOSE###
To leverage existing NRCS technology to improve the collection and distribution of practice certification data in the field


###TECHNOLOGY###
Using the Trimble GeoXT with CartoPac provides the NRCS with a platform for improved field collection by:
- Integrating ArcMap with the GPS device
- Creating custom collection interfaces
- Utilizing databases for advanced querying and reporting
- Standardizing data formats
- Improving data collection and distribution efficiency
#Practice Certification:#
##Trimble GPS Field Collection with CartoPac##


###PURPOSE###
To leverage existing NRCS technology to improve the collection and distribution of practice certification data in the field


###TECHNOLOGY###
Using the Trimble GeoXT with CartoPac provides the NRCS with a platform for improved field collection by:

- Integrating ArcMap with the GPS device
- Creating custom collection interfaces
- Utilizing databases for advanced querying and reporting
- Standardizing data formats
- Improving data collection and distribution efficiency


###PRACTICE CERTIFICATION COLLECTION###
The CartoPac solution for practice certification provides users with the ability to collect point, line, and polygon data types and attribute corresponding practices.

- Each data type can be attributed with feature notes and a dropdown selection input for practice type 
- Only applicable practice types can be selected for the corresponding data type
- The line data type is 3D with each line vertex collecting the northing, easting, and elevation


###GPS COLLECTION INTERFACE###
CartoPac provides the Trimble GPS with a simple custom interface for practice certification.

- Collect a feature
- Select a data type: Point, Line, or Polygon
- Collect field points to build the practice feature shape
- Once the feature’s points are collected, attribute the practice’s code with additional notes
- Practice certification collection is complete


###PRACTICE METADATA###

__PracticePoint__

- OBJECTID: Unique Identifier
- SHAPE: Geometry coordinate values
  - XY point vertex in meters: UTM Zone 12 NAD 83
- PracticeCode: Coded Value Text Field
  - Practice Code
  - Practice Description
- Notes: Text Field – 254 characters


__PracticeLine__

- OBJECTID: Unique Identifier
- SHAPE: Geometry coordinate values
  - XYZ point vertices in meters: UTM Zone 12 NAD 83
- PracticeCode: Coded Value Text Field
  - Practice Code
  - Practice Description
- Notes: Text Field – 254 characters
- Length_Feet_2D: Double Precision Number in Feet
  - Calculates line length without elevation consideration
- Length_Feet_3D: Double Precision Number in Feet
  - Calculates line length with elevation consideration
- SHAPE_Length: Double Precision Number in Meters
  - Length in meters: UTM Zone 12 NAD 83


__PracticePolygon__

- OBJECTID: Unique Identifier
- SHAPE: Geometry coordinate values
  - XYZ point vertices in meters: UTM Zone 12 NAD 83
- PracticeCode: Coded Value Text Field
  - Practice Code
  - Practice Description
- Notes: Text Field – 254 characters
- Area_Acres_2D: Double Precision Number in Acres
  - Calculates area without elevation consideration
- Area_Acres_3D: Double Precision Number in Acres
  - Calculates area with elevation consideration
- SHAPE_Length: Double Precision Number in Meters
  - Perimeter Length in meters: UTM Zone 12 NAD 83
- SHAPE_Area: Double Precision Number in Square Meters
  - Area in square meters: UTM Zone 12 NAD 83
