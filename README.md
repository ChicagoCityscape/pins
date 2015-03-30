# Cook County PINs

This repository contains *two lists of PINs*, or property index numbers. 

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
* [Download a list of 149,750 PINs](https://github.com/ChicagoCityscape/pins/blob/master/missing_parcel_pins_155746.csv.zip) (just the PIN)
* Download PIN data (PIN and metadata)

## Notes
[1] The FOIA request to the Cook County Treasurer's office was considered voluminous and would cost money; the original response said that 50 PINs would fit on a page, making for over 36,000 pages. We inquired about the possibility of providing it in an Excel spreadsheet. The final request was returned in 11 Excel documents after transmitting $100. It was noted in the FOIA request that it was for a commercial use – this extends the time the office has to respond from 5 days to 25 days. 
