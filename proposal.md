# Proposal for Group 108

## Motivation and Purpose
Feeling safe in a neighboorhood is important to quality of life. If we can understand where crime is occuring in a city and the seasonal trends of crime, we can make decisions about where to live and take proetctive measures on our property to minimize the risk of victimization. To assist citizens in this understanding, this data visualization app will allow the public to explore crime trends compared across vancouver neighboorhoods and see the crime trends within specific neighboorhoods of interest.

## Description of the Data
The dataset that we choose to visualize is a public dataset that can be downloaded from the Vancouver Police Department's Open Data: https://geodash.vpd.ca/opendata/. It is a collection of types, locations, dates and times of crimes occurred in City of Vancouver for the past 16 years.  The earliest date in the dataset is January 1, 2003, and the latest date is October 31, 2019.  
  
This dataset is available to the public and no special permit or registration is required.  As it contains temporal-spatial information of crimes, it can be a great guidance to policy makers for laying out community development plans.  As an individual living in Vancouver like ourselves, it can also serve as a reference for selecting residence.

There are 622,221 crime records in this dataset, and each crime record contains: (`TYPE`, `YEAR`, `MONTH`, `DAY`, `HOUR`, `MINUTE`, `HUNDRED_BLOCK`, `NEIGHBOURHOOD`, `X`, `Y`) columns . (`TYPE`) specifies 11 types of crimes (‘Break and Enter Commercial', 'Break and Enter Residential/Other', 'Homicide', 'Mischief', 'Offence Against a Person', 'Other Theft', 'Theft from Vehicle', 'Theft of Bicycle', 'Theft of Vehicle', 'Vehicle Collision or Pedestrian Struck (with Fatality)', 'Vehicle Collision or Pedestrian Struck (with Injury)'), and (`YEAR`, `MONTH`, `DAY`, `HOUR` and `MINUTE`) columns specify the date and time when the reported crime occurred.  To indicate the location of the crimes, we have (`HUNDRED_BLOCK` and `NEIGHBORHOOD`).  (`X` and `Y`) provides the coordinates in UTM Zone 10 format and will need to be converted into longitude and latitude if we want to render a map with GeoJSON.

## Research questions and usage scenarios

### Research questions

- Which neighbourhood should a person from outside Vancouver look for housing?
- Which neighbourhood should a person from within Vancouver look for housing?
- When and where the Vancouver Police Department should have more police portals?

### Usage scenarios

1. Chief of the Vancouver Police Department

    The Chief of the Vancouver Police Department wants to manage the police portals more efficiently to let police portals get to the crime scene as soon as possible. The Chief wants to be able to choose different districts(neighborhoods) in a dataset to compare the crime type and locations in different periods and find the most effective way of arranging the police portals. When the Chief logs on to the "Vancouver Crime Buster App”, an overview of all neighborhoods with all kinds of crimes showed up. The Chief can filter out neighborhoods and different times. So when the Chief compares with the police portals schedule and locations, Chief can make adjust them accordingly. After the Chief did that, the Vancouver Police Department can go to the crime scene faster compared to the past. his app makes the Vancouver Police Department work more efficiently.