# Cleaned-up GTFS feed for Delhi

## Download data

* <https://ethanc8.github.io/delhi-gtfs/bus.zip>
* <https://ethanc8.github.io/delhi-gtfs/metro.zip>

## Changes from source data

* The bus data now expires on 2027-01-01, since we still have realtime data for buses
  * Even the official published timetables were never accurate
  * The realtime data cannot be used without a static feed
* The route IDs for the Metro have been consolidated, the route names are changed to be more user-friendly, and the route colors have been added
  * The colors were taken from [the INAT map of Delhi](https://www.inat.fr/metro/delhi/), since the colors are similar to the official map but are more distinct and work better together.

## Source data

* OTD bus data (OTD/GTFS.zip)
  * Includes DIMTS and DTC buses
  * Source: https://otd.delhi.gov.in/data/static/
  * Expiration date: 2025-01-01 **expired**
* OTD metro (DRMC) data (OTD/DMRC_GTFS.zip)
  * Includes Delhi Metro, Noida Metro, Rapid Metro Gurgaon
  * Does not include Delhi Metro feeder buses
  * Source: https://otd.delhi.gov.in/data/staticDMRC/
  * Expiration date: 2025-12-31

## Realtime data

This GTFS feed is designed to work well with the OTD realtime bus data.
