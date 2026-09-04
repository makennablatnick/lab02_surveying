This readme file was generated on 2026-09-03

# GENERAL INFORMATION

## Title of Dataset: Lab 02 - Surveying - Green

## Contacts:

Name: Wyatt Conger,
Institution: Colorado School of Mines,
Email: wyatt_conger@mines.edu

Name: Makenna Blatnick,
Institution: Colorado School of Mines,
Email: makenna_blatnick@mines.edu

Name: Isaac Peck,
Institution: Colorado School of Mines,
Email: isaac_peck@mines.edu

Name: Isidor Børresen-Jankov,
Institution: Colorado School of Mines,
Email: isidor_borresen-jankov@mines.edu

## Date of data collection: 2026-09-01
## Geographic location of data collection: 
Kafadar Commons, Golden, CO, United States of America

## Information about funding sources that supported the collection of the data: 
Conducted as a part of the GPGN318 coursework

# DATA & FILE OVERVIEW

## File List:

### setup_log.ipynb
- A document summarizing how the grid was set up and how the data was aquired.

### Garmin Data.csv
- produced by GARMIN GPSMAP 67i
- covers every flag in the grid
- collected on 09/01/2026 at around 2:30 PM
- It contains UTM coordinates with meter units
- The first column attempts to replicate the naming scheme of some other groups for each flag location
- The second column is each flag in our naming convention
- The third column represents the zone and band that the UTM coordinates are in
- The fourth column represents the Easting part of the coordinates
- the final column represents the Northing part of the coordinates
- We collected this data as a team
- The only really problematic part of this data is that the data are missing elevations at each of the locations

### green.csv
- Produced by Trimble R10 and the Emlid Reach
- Covers the green flags (Row 1 in our naming convention)
- collected on 09/01/2026 at around 3:00 PM
- it contains UTM coordinates with all units in meters
- Column 1 represents the location
    - "BASE" is the well base station
    - "1" is location A1 and it increments Northward with "5" being location E1
- Column 2 represents the Easting
- Column 3 represents the Northing
- Column 4 represents the elevation (also in meters)
- We collected this data as a team
- Only potential problematic part of this data would be the less than 1 cm difference between the R10 and the actual flag location

### Total_green.csv
- Produced by Trimble C5 Total Station
- Covers the green flags (Row 1 in our naming convention)
- collected on 09/01/2026 at around 3:30 PM
- it contains UTM coordinates with all units in meters
- Column 1 represents the location
   - "E1" is location A1 and it increments North with each point with "E7" being location E1"
   - Locations "E5" and "E6" both represent location D1, so location "E5" should be ignored
- Column 2 represents the Easting
- Column 3 represents the Northing
- Column 4 represents the elevation (also in meters)
- We collected this data as a team
- The only known problems are the one stated above in the column 1 section with the repeat point and the fact that the data skips what would be location E3
    - It is worth noting that while Column 1 skips what would be location E3, all the green flags are documented

