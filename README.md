
# QSS20 NYC Commute Project

##Project Website

[My Website:] https://ballasy27-spec.github.io/QSS20-NYC-Commute/

the project analyzes the differences in commuting burden between Bronx and Manhattan census tracts using 2015 Community Survey data.

## Research Question

Do Bronx census tracts experience longer commute times than Manhattan census tracts even though public-transit use is almost the same?

## Data

The data comes from the U.S. Census Bureau's 2015 American Community Survey 5-year estimates at the census-tract level.

The analysis mainly focuses on:

- Average commute time
- Public-transit use
- Median household income
- Poverty
- Unemployment
- Work from home

## Notebooks

### [00_pull.ipynb](code/00_pull.ipynb)

**Input:** U.S. Census Bureau 2015 ACS 5-year API

Pulls the 2015 ACS census-tract data for New York City from the U.S. Census Bureau.

**Output:** `data/acs2015_nyc_tracts_raw.csv`

### [01_clean.ipynb](code/01_clean.ipynb)

Cleans up the ACS data, keeps Bronx and Manhattan census tracts, removes invalid observations, and creates the final analysis sample.

**Output:** `data/acs2015_bronx_manhattan_clean.csv`

### [02_analyze.ipynb](code/02_analyze.ipynb)

Calculates borough-level summary statistics and compares commute time and public-transit use between the Bronx and Manhattan.

**Outputs:**

- `output/mean_commute_by_borough.png`
- `output/transit_use_by_borough.png`
- `output/borough_summary.csv`

## Main Finding

Bronx and Manhattan census tracts have similar levels of public-transit use, but Bronx census tracts have longer average commute times.
