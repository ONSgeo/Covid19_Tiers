# Covid 19 local restriction tiers by area


Lookups for 2020 Local Authority Districts (also known as Lower Tier Local Authorities) to their respective local restriction tier and for postcodes that contain UPRNs in different Local Authorities.


Lookups produced:
# England (effective 19/12/2020, announced 17/12/2020)
- Lookup: https://github.com/ONSgeo/Covid19_Tiers/blob/main/England_LAD_Covid_Tiers_Effective_19_12_2020.zip[
- Published list: https://www.gov.uk/guidance/full-list-of-local-restriction-tiers-by-area
- Published areas were a mix of different geographies. We have used the smallest geographic unit all areas listed had in common – Local Authority Districts – to create this lookup
- Boundaries that correspond to the 2020 areas and codes can be found: https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=name&tags=all(BDY_LAD%2CMAY_2020)

# England (effective 16/12/2020, announced 14/12/2020)
- Lookup: https://github.com/ONSgeo/Covid19_Tiers/blob/main/England_LAD_Covid_Tiers_Effective_16_12_2020.zip
- Published list: https://www.gov.uk/guidance/full-list-of-local-restriction-tiers-by-area
- Published areas were a mix of different geographies. We have used the smallest geographic unit all areas listed had in common – Local Authority Districts – to create this lookup
- Boundaries that correspond to the 2020 areas and codes can be found: https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=name&tags=all(BDY_LAD%2CMAY_2020)

# England (effective 02/12/2020, announced 26/11/2020)
- Lookup: https://github.com/ONSgeo/Covid19_Tiers/blob/main/England_LAD_Covid_Tiers_Effective_02_12_2020.zip
- Published list: https://www.gov.uk/guidance/full-list-of-local-restriction-tiers-by-area
- Published areas were a mix of different geographies. We have used the smallest geographic unit all areas listed had in common – Local Authority Districts – to create this lookup
- Boundaries that correspond to the 2020 areas and codes can be found: https://geoportal.statistics.gov.uk/search?collection=Dataset&sort=name&tags=all(BDY_LAD%2CMAY_2020)

# Split Postcodes in England and thier Tiers (effective 02/12/2020)
-	Some postcodes in England straddle the border of multiple Local Authorities. This lookup provides a list of those postcodes (which represent around 1% of all postcodes in England). In theory this means different parts of a postcode could be in different tiers if it crosses between Local Authorities with different restrictions. This lookup suggests just under 0.1% of postcodes in England are split to some extent between different tiers. However, there are caveats around this value which are explained below which mean this value should be considered an upper estimate. 
- Lookup: https://github.com/ONSgeo/Covid19_Tiers/blob/main/England_Split_PCD_Covid_Tiers_Effective_02_12_2020.csv
- What the different columns mean:
  > N_UPRNS – Number of UPRNs in the postcode/local authority combination </br>
  > UPRN_PROP – Proportion of UPRNs in that postcode/local authority combination over postcode total </br>
  > UPRN_PROP_RANK – Ranked UPRN_PROP  with 1 being the largest proportion </br>
  > TIER – Tier that the local authority is in (effective 02/12/2020) </br>
  > TIER_DIFF – Flag 0 if there is no difference in tier assignment in the postcode and Flag 1 if tiers are different for that postcode
- An important caveat with this lookup. We have used the <a href="https://geoportal.statistics.gov.uk/datasets/ons-uprn-directory-october-2020">October 2020 ONS UPRN Directory</a> to create this lookup. This contains all UPRNs in Great Britain – not just UPRNs where people live. As such, this means there are likely to be instances in this lookup where we say a postcode is split, but this may in fact be caused by the inclusion of non-residential UPRNs. We could have only included UPRNs where we believe people live based on the data available in <a href="https://www.ordnancesurvey.co.uk/business-government/products/addressbase">Ordnance Survey’s AddressBase</a> product. However, if we had done this we would have been unable to release the resulting lookup as open data.
