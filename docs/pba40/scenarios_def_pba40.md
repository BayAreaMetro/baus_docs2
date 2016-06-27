# PBA40 Draft Scenario Definition

## Concise Scenario Comparion

   S    |             0             |             1             |             2             |            3              |            4              |            5
------- | ------------------------- | ------------------------- | ------------------------- | ------------------------- | ------------------------- | -------------------------           
**Zoning** | [existing](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/zoning_mods_0.csv) | upzone select PDAs        | upzone PDAs to placetype  | upzone TPAs in Big3 and neighbors | upzone some PDAs | ttt
**UGB** | expand by 389 sq mi | expand by 565 sq mi | existing UGBs/city limits add 68 sq mi | city boundaries | existing UGBs/city limits add 68 sq mi | ttt 
**Caps** | existing | existing | raises SF OF cap to 1.5m | drops SF OF cap | existing | ttt 
**DevProj** | where scen0=1 | where scen1=1 | where scen2=1 | where scen3=1 | where scen4=1 | ttt                         
**Sec Units** | *existing* | *everywhere* | *pdas* | *in big 3* | *pdas* | ttt
**SubFee** | [sb743](accounts_pba40.md#sb743) | [inclusionary-low](accounts_pba40.md#inclusionary-zoning-low) <br> [parceltax](accounts_pba40.md#parcel-tax) <br> [hu_capgains](accounts_pba40.md#housing-capital-gains-tax) <br> [obag](accounts_pba40.md#obag) <br> [tiering](accounts_pba40.md#ceqa-tiering) <br> [sb743](accounts_pba40.md#sb743) | [inclusionary-medium](accounts_pba40.md#inclusionary-zoning-medium) <br> [obag](accounts_pba40.md#obag) <br>  [tiering](accounts_pba40.md#ceqa-tiering) <br> [sb743](accounts_pba40.md#sb743) | [inclusionary-high](accounts_pba40.md#inclusionary-zoning-high) <br> [obag](accounts_pba40.md#obag) <br> [tiering](accounts_pba40.md#ceqa-tiering) <br> [sb743](accounts_pba40.md#sb743) | ttt | ttt 
**VMT Fee** | none | [com](accounts_pba40.md#vmt-fees) | NA | [res](accounts_pba40.md#vmt-fees) | NA | ttt
**Pkg Mins** | existing | decreased in pdas along rail | decreased in core pdas | decreased in big 3 and neighbors | decreased in core pdas | ttt
**Tax** |  |  | | [land value tax in big 3 and neighbors](accounts_pba40.md#land-value-tax) | ttt | ttt                        
**Net** |                           |                           |                           | | ttt | ttt               
                         
                         


## Scenario 0 (the No Project)

* [zoning_mods_np](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/zoning_mods_0.csv) expands suburban area by 389 sq miles (ubz, ubz_np, exp0, exp0_np, exp1, exp1_np, and exp2_np are upzoned)
* keeps existing 2010 jurisdictional development caps
* second units allowed in jurisdictions that allow in 2010 (not implemented yet)
* residential parking minimums as in 2010
* SB743: To represent the EIR move from LOS to VMT, we want to do a slight "subsidy" in efficient VMT locations and a slight penalty in inefficient ones. Can we do %? Or we could translate into something like the VMT fee with absolute amounts. If % possible try as in SB743 Profitability Modification Table below
* builds projects where scen0=1 in [Development Projects](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/development_projects.csv). These are 1) projects built between 2010 and 2015, and 2) large institutional projects started by 2015
* committed transportation network/policies

## Scenario 1

* TODO: more emp movement to suburban subcenters
* [zoning_mods_au](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/zoning_mods_au.csv) upzones select suburban centers (res and com) and expands UGBs "faster than expected compared to past trends" so expands suburban area by 565 sq miles  (ubz, exp0, exp1, exp3_au, and expmaz(79sqmi) are upzoned while avoiding PCAs)
* keeps existing 2010 jurisdictional development caps
* second units allowed in all jurisdictions (not implemented yet)
* residential parking minimums decreased in PDAs along rail
* SB743 as in scen0
* OBAG: In 2010 one account is set up for the entire region. Each year $200m is added to the account. In a given year, whatever is in the account is available to subsidize housing construction within any PDA in the region.
* inclusionary housing policy in jurisdictions with at least one PDA that taxes new housing construction to subsidize affordable housing construction within that jurisdiction.
* vmt_fee_com assesses fees on office and retail construction in zones where employees have high average commute lengths. Zones are classified according to the variable nonres_cat in [vmt_fee_zonecats.csv](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/vmt_fee_zonecats.csv).
* builds projects where scen1=1 in [Development Projects](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/development_projects.csv). These are 1) projects built between 2010 and 2015, and 2) large institutional projects started by 2015
* scenario 1 network/policies


## Scenario 2

* [zoning_mods_pr](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/zoning_mods_2.csv) upzones PDAs to match their place type and assumes 2010 UGBs hold (existing true UGB/ULL and city boundaries where no limit) (ubz only while avoiding PCAs) so 68 additional sq miles
* keeps existing 2010 jurisdictional development caps except raises SF office cap to 1.5m annually
* second units along all jurisdictions along El Camino Real and East Bay Corridors (not implemented yet)
* residential parking minimums decreased in PDAs that have high levels of transit access along El Camino Real and East Bay Corridors
* SB743 as in scen0
* OBAG as in scen1
* inclusionary housing policy in jurisdictions with at least one PDA that taxes new housing construction to subsidize affordable housing construction within that jurisdiction. 
* builds projects where scen2=1 in [Development Projects](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/development_projects.csv). These are 1) projects built between 2010 and 2015, and 2) large institutional projects started by 2015 
* scenario 2 network/policies


## Scenario 3

* TODO: more emp in big 3, more housing in oakland
* [zoning_mods_th](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/zoning_mods_3.csv) upzones areas with high transit access (with an emphasis on the Big 3 and their neighbors) and tightens UGBs to city boundaries
* keeps existing 2010 jurisdictional development caps except drops SF office cap
* second units allowed in Big 3 cities (not implemented yet)
* residential parking minimums decreased in Big 3 cities and neighboring high transit cities 
* SB743 as in scen0
* OBAG as in scen1
* inclusionary housing policy in Big 3 Cities that taxes new housing construction to subsidize affordable housing construction within that jurisdiction.
* tax policy: land value tax in Big 3
* vmt_fee_res assesses fees on residential construction in zones with households with high average commute lengths. Zones are classified according to the variable res_cat in [vmt_fee_zonecats.csv](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/vmt_fee_zonecats.csv).
* builds projects where scen3=1 in [Development Projects](https://github.com/MetropolitanTransportationCommission/bayarea_urbansim/blob/master/data/development_projects.csv). These are 1) projects built between 2010 and 2015, and 2) large institutional projects started by 2015, and 3) very large mixed-use projects that have been designed and assessed for feasibility using spreadsheet pro formas 
* scenario 3 network/policies


## Scenario 4 (the Preferred Plan)
* all directions in writing from Cynthia only
* 98% of what want for res
* Santa Rosa too much housing (placetypes wrong)


## Scenario 5
* placeholder likely for use with autonoumous vehicles assessment
