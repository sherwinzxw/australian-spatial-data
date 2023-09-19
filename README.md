# Australian Spatial Data - TopoJson 
A repository of the simplified TopoJSON data that encodes the Australian Commonwealth, States, and Territories for high performing shapre map generation use.

## Description

This repository uses the open-source [Digital Boundary Files](https://www.abs.gov.au/statistics/standards/australian-statistical-geography-standard-asgs-edition-3/jul2021-jun2026/access-and-downloads/digital-boundary-files) datasets from the Australian Bureau of Statics (ABS) 

#### Preview on map
![image](https://github.com/sherwinzxw/australian-spatial-data/assets/12377619/b29a4547-ab41-4f91-b1b6-6b220728eec4)
* You can find the map preview at [here](https://github.com/sherwinzxw/australian-spatial-data/blob/master/data/spatial_data/states/vic/topojson/simplified/POA_2021_VIC_GDA2020.json)
* Due to BING map area code support and data rendering size issues, only a few Postal Areas map previews are enabled.

#### Available TopoJSON datasets
Please find below for the list of avaiable TopoJSON datasets:
* Commonwealth level
   * Australia map
   * Commonwealth Electoral Divisions (CED) map
   * Greater Capital City Statstical Areas (GCCSA) map
   * Local Government Areas (LGA) map
   * Postal Areas (POA) map
   * Suburbs and Localities (SAL) map
   * State Electoral Divisions (SED) map
   * State and Territories (STE) map  
* State/Territory level
   * Commonwealth Electoral Divisions (CED) map
   * Greater Capital City Statstical Areas (GCCSA) map
   * Local Government Areas (LGA) map
   * Postal Areas (POA) map
   * Suburbs and Localities (SAL) map
   * State Electoral Divisions (SED) map

#### About the ABS Postal Areas boundary data
The Postal Areas boundary data is encoded with Australian postal code as the row key, and this row key has not been associated with any Austrlian states or territories. \
As a result, I have apply partition transformation to the postal codes according to the postcode ranges defined by the [Australia Post](https://www.auspost.com.au), which by law manages the lifecycle of Australian postcodes. \
Please see below for the postcode ranges for each state/territory: 
<table>
   <thead>
      <tr>
         <th>State/Territory</th>
         <th>Postcode Range(s)</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>New South Wales</td>
         <td>1000-2599, 2620-2899, 2921-2999</td>
      </tr>      
      <tr>
         <td>Victoria</td>
         <td>3000-3999, 8000-8999</td>
      </tr>      
      <tr>
         <td>Queensland</td>
         <td>4000-4999, 9000-9999</td>
      </tr>      
      <tr>
         <td>South Australia</td>
         <td>5000-5999</td>
      </tr>      
      <tr>
         <td>Western Australia</td>
         <td>6000-6999</td>
      </tr>      
      <tr>
         <td>Tasmania</td>
         <td>7000-7999</td>
      </tr>      
      <tr>
         <td>Australian Capital Territory</td>
         <td>0200-0299, 2600-2619, 2900-2920</td>
      </tr>      
      <tr>
         <td>Northern Territory</td>
         <td>0800-0999</td>
      </tr>
   </tbody>
</table>


## Author
Xinwei (Sherwin) Zhao

## Version History
* 0.1
    * Initial Release

## Acknowledgments

Greate thanks to below source data and service providers
* [Australian Bureau of Statistics](https://www.abs.gov.au/)
* [Australia Post](https://www.auspost.com.au)
* [Matthew Proctor](https://www.matthewproctor.com)
* [Mapshaper](https://github.com/mbloch/mapshaper)
