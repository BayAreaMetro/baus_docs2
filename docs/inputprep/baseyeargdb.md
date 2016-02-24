# Base Year GeoDatabase

Bay Area UrbanSim requires a representation of the region's parcels, buildings, households, and employees for the base simulation year (2010). This data is pulled together, integrated, and clean up using a series of scripts originally writen by [UDST](https://udst.org) 

## Computing Environment, Setup, and Configuration for Base Year GeoDatabase Cleaning


## Running the Script

set of steps

The steps below follow the code residing [here](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/tree/master/data_regeneration) 

### Load and Clean County Parcel Files

### County-Specific Cleaning

### Merge the County Parcels into a Regional Parcel Database

### Merge Parcels for Condos, Common Areas, and Stacked Duplicate Parcels

### Fill In Missing Values Using xxxx

### Tag Parcels with zone_id

Tags parcels with TAZ (zone) ID using [point-in-poly](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data_regeneration/spatialops.py#L10) or [closest](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data_regeneration/spatialops.py#L14) when parcel falls outside the TAZ map.


### Match Aggregate

### Impute Prices

### Allocate Demand Agents to Buuldings

### Perform Quality Control Summaries

### Export Integrated Parcels
The [export_to_h5](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data_regeneration/export_to_h5.py) script:

* [maps](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data_regeneration/export_to_h5.py#L15-L31) development_type_id to building_type_id

* sets the h5 [path](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data_regeneration/export_to_h5.py#L13)

* [stores](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data_regeneration/export_to_h5.py#L60-L67) the tables in the hdf5

* among other things 

