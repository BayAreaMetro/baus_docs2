# Subsidies, Fees, and Other Policies Represented by Accounts/Profit Modification

## SB743
(Modification, Applied regionwide by TAZ) This refelcts the expected shift in CEQA transporation analysis requirements from emphasising LOS to emphasizing VMT. Project profitabilility shifts as in the table below.

### SB743 Profitability Modification Table
| vmt_cat (res or non_res) | profitability shift |
|--------------------------|---------------------|
| VH                       | -2%                 |
| H                        | -1%                 |
| MH                       | -0.5%               |
| M                        | 0                   |
| S                        | +2%                 |


## OBAG 
(Account, Applied to all PDAs) $160 million per year is spent on projects within the PDAs. Although this funds planning and infrastructure projects, we treat it here as a direct subsidy as if the developer received an equivalent amount of money to build a project.


## CEQA Tiering 
(Modification, Applied to all TPAs)
Make any sort of development in a TPA 1% more profitable


## Parcel Tax
(Account, Applied to all PDAs, Deed-Restricted)
$24 annual parcel tax throughout region into fund for affordable housing
so $42,000,000 is placed in an account annually to be spent on affordable housing in any PDA in the region 


## Housing Capital Gains Tax
(Account, Applied to all PDAs, Deed-Restricted)
$500,000,000 is placed in an account annually to be spent on affordable hosuing in any PDA in the region


## No Parking Minimums  
(Modification, Applied to PDAs in 1 and 2, TPAs in 3)
Make projects 1% more profitable in zone above. (Or is there a better proxy from the parking work? or other research?)

## Inclusionary Zoning Low
(Account, Applied to all Opportunity Jurisdiction, Deed-Restricted)
Sets a low level of inclusionary units requried with a proportion required of 0.05 for these jurisdictions: 
Alameda
Alameda County
Albany
American Canyon
Antioch
Atherton
Belmont
Benicia
Berkeley
Brisbane
Burlingame
Campbell
Cloverdale
Colma
Concord
Contra Costa County
Cotati
Cupertino
Daly City
Danville
Dixon
Dublin
East Palo Alto
El Cerrito
Emeryville
Fairfield
Foster City
Fremont
Gilroy
Hayward
Hercules
Lafayette
Lake County
Livermore
Los Altos
Los Altos Hills
Los Gatos
Martinez
Menlo Park
Millbrae
Milpitas
Monte Sereno
Moraga
Morgan Hill
Mountain View
Napa
Newark
Oakland
Oakley
Orinda
Palo Alto
Petaluma
Piedmont
Pinole
Pittsburg
Pleasant Hill
Pleasanton
Redwood City
Richmond
Rohnert Park
Sacramento County
San Benito County
San Bruno
San Carlos
San Francisco
San Francisco County
San Joaquin County
San Jose
San Leandro
San Mateo
San Mateo County
San Pablo
San Rafael
San Ramon
Santa Clara
Santa Cruz County
Santa Rosa
Saratoga
Sebastopol
South San Francisco
Stanislaus County
Suisun City
Sunnyvale
Union City
Vacaville
Vallejo
Walnut Creek
Windsor
Yolo County

## Inclusionary Zoning Medium
(Account, Applied to Jurisdictions with PDAs, Deed-Restricted)
Sets a moderate level of inclusionary units requried with a proportion required of 0.1 for these jurisdictions: 
Alameda
Alameda County
Albany
American Canyon
Antioch
Belmont
Benicia
Berkeley
Brisbane
Burlingame
Campbell
Cloverdale
Colma
Concord
Contra Costa County
Cotati
Cupertino
Daly City
Danville
Dixon
Dublin
East Palo Alto
El Cerrito
Emeryville
Fairfield
Fremont
Gilroy
Hayward
Hercules
Lafayette
Lake County
Livermore
Los Altos
Martinez
Menlo Park
Millbrae
Milpitas
Moraga
Morgan Hill
Mountain View
Napa
Newark
Oakland
Oakley
Orinda
Palo Alto
Petaluma
Piedmont
Pinole
Pittsburg
Pleasant Hill
Pleasanton
Redwood City
Richmond
Rohnert Park
Sacramento County
San Benito County
San Bruno
San Carlos
San Francisco
San Francisco County
San Joaquin County
San Jose
San Leandro
San Mateo
San Mateo County
San Pablo
San Rafael
San Ramon
Santa Clara
Santa Cruz County
Santa Rosa
Sebastopol
South San Francisco
Stanislaus County
Suisun City
Sunnyvale
Union City
Vacaville
Vallejo
Walnut Creek
Windsor
Yolo County


## Inclusionary Zoning High
(Account, Applied to Big 3 Cities and Neighbors, Deed-Restricted)
Sets a relatively high level of inclusionary units requried with the proportion required in each jurisdiction listed here:
###inclusionary_housing_high

| juris         | prop |
|---------------|------|
| San Francisco | 0.2  |
| Oakland       | 0.2  |
| San Jose      | 0.2  |


## VMT Fees
(Account, Applied regionally by TAZ, Deed-Restricted)

The fees in the table below are assessed on development in zones with higher VMT (home-end of commute for res; work-end of commmute for commercial. Res assessed on any type of residential development; commercial only for office and retail. Money available regionally to subsidize housing construction in Zone S. Susidized units are deed-restricted.

### VMT Fees by Zone Category Table

| Category| Residential VMT Fee Action          |Commercial VMT Fee Action             |
|---------|-------------------------------------|--------------------------------------|
| VH      | assess res dev fee $25,000 per HU   | assess com dev fee $20 per OF/RS sqft|
| H       | assess res dev fee $15,000 per HU   | assess com dev fee $10 per OF/RS sqft|
| MH      | assess res dev fee $5,000 per HU    | assess com dev fee $6 per OF/RS sqft |
| M       | nothing                             | nothing                              |
| S       | money available to subsidize units  | money available to subsidize res units|
 
 
## Land Value Tax
(Modification, Applied to Big 3 cities)
In the Big 3 cities, represent approximate impacts of switching from the current property tax system to one which achieves the same income but only from taxing the value of the land value (and not the structure value). Could we approach this: every so many more percent lower the improvement-to-land ratio is, profitability on a new structure rises some percent? For now lets try assuming an acre of land is worth $33.3m in SF, $7.8m in San Jose, and $5.4m in Oakland and apply these changes to land zoned for HM:

| ILR     | Residential Profitability Change    |Commercial Profitablity Change        |
|---------|-------------------------------------|--------------------------------------|
| > 0.5    | no change                           | no change                            |
| 0.5-0.3 | 1%                                  | 1%                                   |
| 0.3-0.1 | 2%                                  | 2%                                   |
| < 0.1    | 5%                                  | 5%                                   |
