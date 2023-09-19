# Australian Spatial Data - TopoJson 
A repository of the simplified TopoJSON data that encodes the Australian Commonwealth, States, and Territories for high performing shapre map generation use.

## Description

This repository uses the open-source [Digital Boundary Files](https://www.abs.gov.au/statistics/standards/australian-statistical-geography-standard-asgs-edition-3/jul2021-jun2026/access-and-downloads/digital-boundary-files) datasets from the Australian Bureau of Statics (ABS) 

#### Preview on map
![image](https://github.com/sherwinzxw/australian-spatial-data/assets/12377619/b29a4547-ab41-4f91-b1b6-6b220728eec4)
* You can find the map preview at [here](https://github.com/sherwinzxw/australian-spatial-data/blob/master/data/spatial_data/states/vic/topojson/simplified/POA_2021_VIC_GDA2020.json)
* Due to BING map area code support and data rendering size issues, only a few Postal Areas map previews are enabled.

### About the ABS Postal Areas boundary data
The Postal Areas boundary data is encoded with Australian postal code as the row key, and this row key has not been associated with any Austrlian states or territories.
As a result, I have apply grouping transformation to the postal codes according to the postcode ranges defined by the [Australia Post](https://www.auspost.com.au).

## Author
Xinwei (Sherwin) Zhao

## Version History
* 0.1
    * Initial Release

## Acknowledgments

Greate thanks to below source data and service providers ()
* [Australian Bureau of Statistics](https://www.abs.gov.au/)
* [Australia Post](https://www.auspost.com.au)
* [Matthew Proctor](https://www.matthewproctor.com)
* [Mapshaper](https://github.com/mbloch/mapshaper)
