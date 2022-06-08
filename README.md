# senatedist24
Minnesota Senate District 24 Data Analysis

## Datasets

- "MnRegisteredVoterCountsByPrecinctJune2021.csv"
    - Number of registered voters by precinct for all precincts in MN as of June 1, 2021
    precinct
    - From MN SOS: https://www.sos.state.mn.us/election-administration-campaigns/data-maps/voter-registration-counts/
    - Will be updated June 1, 2022
    - Note: there is more than 1 entry for each precinct (since precincts also split by school dist, etc)


- "18PlusVotersByVotingDistrictInDodgeOlmsteadCounties.csv"
    - Dataset of 18+ voters by race by each voting district(precinct) for all precincts in Olmstead and Dodge county.
    - From Census.gov: https://data.census.gov/cedsci/table?t=Populations%20and%20People%3AVoting%20and%20Registration&g=0500000US27039,27039%247000000,27109,27109%247000000&tid=DECENNIALPL2020.P3&tp=true
    - Also has breakdowns by race if we want to look into that


- "18PlusVotersByVotingDistrictInDodgeOlmsteadCounties_AddedPrecinctCodes_Trimmed.csv"
    - Dataset of 18+ voters by each voting district(precinct) for all precincts in State Sen Dist 24.
    - Same dataset as above but edited:
    1. Includes a column with corresponding precinct codes (Precinct codes from MN SOS dataset)
    2. Only includes total column of all races
    3. Only include precincts in senate dist 24
        - (Ideally we could get the census.gov dataset of 18+ voters by each voting district(precinct) in senate dist 24, but the group of voting dists inside senate districts don't seem to be updated to account for redistricting [https://data.census.gov/cedsci/table?t=Populations%20and%20People%3AVoting%20and%20Registration&g=0500000US27039%247000000_610XX00US27024&tid=DECENNIALPL2020.P3&tp=true] so we're getting voting dists in the 2 counties and manually removing the ones we don't need)
