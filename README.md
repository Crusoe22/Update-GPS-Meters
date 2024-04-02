# Update-GPS-Meters
# Python Code Documentation

This Python script utilizes ArcPy and Pandas libraries to update feature classes within ArcGIS based on information stored in an Excel workbook.

## Requirements
- ArcGIS Pro
- Pandas library for Python
- ArcPy library

## Usage
1. Ensure that ArcGIS Pro is installed on your system.
2. Install the Pandas library if it's not already installed. You can install it using pip: `pip install pandas`.
3. Configure the paths in the script according to your system.
4. Run the script.

## Description
The script performs the following operations:

1. **update_assetID()**: Updates the 'ASSETID' field in the feature class based on matching GIS account numbers from an Excel workbook.
2. **SizefromExcel()**: Updates the 'SIZE' field in the feature class based on matching GIS account numbers from an Excel workbook.
3. **update_meterSize()**: Updates the 'METER_SIZE' field in the feature class based on the 'SIZE' field values.
4. **update_serviceType()**: Updates the 'SERVICETYPE' field based on the 'SIZE' field values.
5. **update_editor()**: Updates the 'Last Editor' and 'Last Update Field' in the feature class.
6. **update_fixed()**: Updates the 'ACCURACY' field in the feature class.
7. **update_accountNum()**: Updates the 'ACCOUNTID' field based on the 'GISACCOUNT' field values.
8. **update_location()**: Calculates geometry attributes such as Latitude, Longitude, Northing, Easting, and Elevation.
9. **update_empty()**: Updates the 'ACCOUNTID' field based on 'Notes' field values.
10. **update_facilityID()**: Updates the 'FACILITYID' field in the feature class.

## Notes
- Ensure that all paths to files and feature classes are correctly specified.
- This script assumes a specific structure and naming convention of fields in the feature class. Adjustments may be needed based on your data schema.
- Before running the script, ensure that appropriate permissions are set to update the feature class.
- It's recommended to review and backup your data before running the script, especially operations that involve updating fields.
