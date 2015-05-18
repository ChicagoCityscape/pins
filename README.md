# Cook County PINs & Townships

This repository contains *two lists of PINs*, or property index numbers. It will eventually contain property taxes data (billed and assessed values for all properties).

1. All Cook County Property Index Numbers billed for 2014
2. Other PINs we know about that aren't in list #1

## What are PINs?
A PIN describes a property, often in the form of a discrete parcel of a land, but frequently as a condo in a shared piece of land. Most of the PINs represent taxable properties; the remainder represent exempt properties, or "retired" PINs that resulted from splitting or joining PINned properties. 

A PIN is 14 digits long and can be divvied into five, meaningful parts. A PIN is most often an integer, but many have leading zeros.

## What's in List #1?
List 1 contains the response to a FOIA request [1], asking for a list of "all PINs" (and its metadata: property address, city, class, and description) that were on the tax roll in 2014. 

* 1,864,384 PINs were received in the FOIA request
* 1,863,813 unique PINs
* XXX is the number of PINs that had records on the Cook County Property Info Portal

### Get the data
* [Download a list of PINs](https://github.com/ChicagoCityscape/pins/blob/master/all_cook_pins_1863813.csv.zip) (just the PIN)
* Download PIN data (PIN and metadata)

## What's in List #2?
List 2 contains 155,746 PINs that are in the [Parcel2012 shapefile](https://datacatalog.cookcountyil.gov/GIS-Maps/ccgisdata-Parcel-2012/e62c-6rz8) from the Cook County data portal but which are not present in List 1 ("all PINs"). 

149,750 is the number of PINS that had records on the Cook County Property Info Portal.

### Get the data
* [Download a list of 155,746 PINs](https://github.com/ChicagoCityscape/pins/blob/master/missing_parcel_pins_155746.csv.zip) (just the PIN)
* Download PIN data (PIN and metadata)

## Property classes and descriptions
When you're analyzing PINs and property taxes it's useful to know the property's class and class description. There are 132 unique classes, including *null* and "unclassified" values. The most common property class is "2-99, Residential condominium".

### Get the data
* [Download a table of classes, descriptions, and property counts](https://github.com/ChicagoCityscape/pins/blob/master/property_class_descriptions.csv)

## Township and township neighborhood boundaries
Townships are tax collecting boundaries and the sub-township neighborhood helps the township assessor asses a property's value. 

This data is a manually-drawn GIS boundary of all of the townships and township neighborhoods within the City of Chicago. Drawing the boundary edges was assisted by the street center lines and other official boundary data. 

### Get the data
* [Download as a zipped shapefile](https://github.com/ChicagoCityscape/pins/blob/master/chicago_townships.zip). Projection is EPSG:3435, Illinois StatePlane East (feet)
* [Download as GeoJSON](https://github.com/ChicagoCityscape/pins/blob/master/chicago_townships.geojson). Projection is EPSG:4326, WGS84 mercator

## Notes
[1] The FOIA request to the Cook County Treasurer's office was considered voluminous and would cost money; the original response said that 50 PINs would fit on a page, making for over 36,000 pages. We inquired about the possibility of providing it in an Excel spreadsheet. The final request was returned in 11 Excel documents after transmitting $100. It was noted in the FOIA request that it was for a commercial use – this extends the time the office has to respond from 5 days to 25 days. 
