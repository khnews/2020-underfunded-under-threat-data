# Underfunded and Under Threat

This repository contains data used in [Underfunded and Under Threat](https://khn.org/news/tag/underfunded-and-under-threat/), a series examining how the U.S. public health front lines have been left understaffed and ill-prepared to save us from the coronavirus pandemic. The project is a collaboration between KHN and the Associated Press.

[Read the main story](https://khn.org/news/us-public-health-system-underfunded-under-threat-faces-more-cuts-amid-covid-pandemic/) and the [continuing series](https://khn.org/news/tag/underfunded-and-under-threat/).

## Overview

On every level, governments have been starving public health for decades. Now, a wave of layoffs and furloughs in some regions further undercutting what remains of limited staffs, complicating efforts to stop the spread of COVID-19.

An analysis by KHN and The AP finds that, since 2010, most state public health departments have slashed per capita spending and staffing. On the local level, median per person spending has declined by nearly 20% overall.

The government tasks public health workers with improving the health of the general population, through their work to encourage healthy living and prevent infectious disease. To that end, public health officials do everything from inspecting water and food safety to testing the nation’s babies for metabolic diseases and contact tracing cases of syphilis.

But investment in public health varies widely by state and county, creating uneven ranks instead of a strong defense, according to the analysis. As COVID-19 cases spike in the wake of reopenings, cuts are increasing as new budgets reflect the financial calamity wrought by the virus.


## Findings

Among the findings:

* Since 2010, spending for state public health departments has dropped by 16% per capita, and for local health departments by 18%. Local public health spending varies widely by county or town, even within the same state.
* At least 38,000 state and local public health jobs have disappeared since the 2008 recession, leaving a skeletal workforce in what was once viewed as one of the world’s top public health systems.
* Nearly two-thirds of Americans live in counties that spend more than twice as much on policing as they spend on nonhospital health care, which includes public health.
- More than three-quarters of Americans live in states that spend less than $100 per person annually on public health. Spending ranges from $32 in Louisiana to $263 in Delaware.
* Some public health workers earn so little that they qualify for government assistance. During the pandemic, many have found themselves disrespected, ignored or even vilified. Dozens of state and local public health leaders have announced their resignations, retired or been fired in 17 states since April.
* States, cities and counties whose tax revenues have declined during the current recession have begun laying off and furloughing public health staffers. At least 14 states have cut health department budgets or positions, or were actively considering such cuts in June, even as coronavirus cases surged in several states.

## Using the Data

This dataset includes a number of files to help you tell this story in your area:

* [01-state-public-health-agencies.csv](data/01-state-public-health-agencies.csv) contains total and per capita data on state-level public health agency full-time equivalent (FTE) staffing and expenditures at multiple points in the past decade
* [02-state-local-government-spending.csv](data/02-state-local-government-spending.csv) contains spending from all state and local governments, rolled up to the state level, by several key categories, including nonhospital health, hospitals, policing and education
* [03-county-local-government-spending.csv](data/03-county-local-government-spending.csv) contains local government spending rolled up to the county level, by several key categories, including nonhospital health, hospitals, policing and education
* [04-local-health-departments-total-by-state.csv](data/04-local-health-departments-total-by-state.csv) contains total spending and FTE staffing from LHDs in Florida, Kentucky. Minnesota, Missouri, North Carolina, Ohio and Washington for all years available
* [05-local-health-departments-detail.csv](data/05-local-health-departments-detail.csv) contains spending and FTE staffing at the LHD level from LHDs in Florida, Indiana, Kentucky, Minnesota, Missouri, North Carolina, Ohio and Washington state for all years available
* [06-state-directory.csv](data/06-state-directory.csv) contains classification of local health departments in each state, based on their state governance, plus a link to each state’s local health department information page. It also contains the percent of each state’s spending that is on public health and the amount per resident.

Column definitions are in [data-dictionary.csv](data-dictionary.csv).

## Methodology and Caveats

### Glossary

- FTE = full-time equivalent worker
- LHD = local health department, such as a county, city or regional health department

LHD jurisdictions vary from single counties to multicounty regions, cities, multicity regions and parts of counties. In addition, the relationships between LHDs and their states vary from completely independent to entirely run by the state. The [Association of State and Territorial Health Officials](https://www.astho.org/) (ASTHO) classifies LHDs in each state by governance, which we’ve included in the [state LHD directory data file](data/01-state-public-health-agencies.csv). You can read more about how they define the categories in ASTHO’s [2016 Profile Report](https://www.astho.org/Profile/Volume-Four/2016-ASTHO-Profile-of-State-and-Territorial-Public-Health/). There are also 12 nationally recognized [Tribal Epidemiology Centers](https://tribalepicenters.org/12-tecs/) and many [tribal health departments](https://www.cdc.gov/tribal/tribes-organizations-health/tribal_groups.html).

### Inflation and Population

All financial data was inflation-adjusted to 2019 using the Bureau of Economic Analysis’ “Government consumption expenditures and gross investment: State and local - implicit price deflator.” The first-quarter value was used for 2020, otherwise annual values were used.

Population data for per capita figures comes from the Census Bureau’s intercensal [population estimates](https://www.census.gov/programs-surveys/popest.html).

### State Public Health Agencies (dataset 1)

Data on state public health agencies’ expenditures and full-time equivalent (FTE) staffing is from the [Association of State and Territorial Health Officials](https://www.astho.org/). The data was reported directly by the state public health agencies through a national survey. For many states, workforce totals include state health agency employees working in local health departments, and expenditure totals include funds passed to local health departments.

When creating national percentage change estimates, we exclude states that do not have comparable data. We exclude Kansas, New Jersey, Texas and Wyoming for percent change in full-time equivalent staffing from 2010 to 2019. We exclude Missouri, Michigan, Texas and Wyoming for percent change in expenditures from 2010 to 2018.

Specific caveats:

* Kansas’ 2010-16 workforce numbers represent the state’s division of public health, while the 2019 numbers represent the entire Department of Health and Human Services.
* Maryland workforce numbers represent the state’s entire Department of Health, but expenditures represent only the public health division of that agency.
* Michigan workforce numbers represent the state public health agency, but the 2019 financial numbers represent the newly merged Department of Health and Human Services (which now includes Behavioral Health Services).
* New Jersey workforce numbers for 2019 are not comparable to previous years.
* Texas’ agency structure changed between the 2016 and 2019 surveys, with the health agency moving out from under a larger umbrella organization to become its own entity.
* Wyoming’s 2010-12 workforce numbers represent the state’s entire Department of Health, but expenditures represent only the public health division of that agency.

### State and Local Government Spending (datasets 2+3)

State and local government total spending is from the [U.S. Census Bureau Annual Survey of State and Local Government Finances](https://www.census.gov/programs-surveys/gov-finances/data/datasets.html), retrieved from the [Urban Institute’s State and Local Finance Initiative](https://state-local-finance-data.taxpolicycenter.org/pages.cfm).

Local government (including county, city, town, etc.) spending for 2017 was rolled up to the county level by the [State Health Expenditure Dataset](http://systemsforaction.org/projects/optimizing-governmental-health-and-social-spending-interactions/tools/state-health-expenditure-dataset-shed-2000-2013) team (with faculty from Johns Hopkins University, the University of Minnesota and Arizona State University).

The state and local government spending data is self-reported and may contain errors. Percent of total is calculated by dividing each expenditure category by total expenditures.

Nonhospital health includes public health, behavioral health, medical transportation and other nonhospital health-related spending. It does not include Medicaid spending.

### Local Health Departments (datasets 4+5 and some national-level findings)

National figures on LHDs are from the National Association of County and City Health Officials’ (NACCHO) [Profile Study](http://nacchoprofilestudy.org/), which surveys local health departments approximately every three years. Individual health department responses are weighted by NACCHO to account for non-response. The AP and KHN used NACCHO data for some national findings summarized above.

The datasets in the distribution on individual LHDs were gathered by KHN from various state agencies, where we were able to obtain comprehensive FTE staffing and/or expenditures data.

We determined the area each LHD serves using information from the state and local agencies, as well as NACCHO. We added NACCHO identifiers to this data for ease of use. Where NACCHO identifiers were not available, we create new identifiers, starting with the number 900.

LHD jurisdictions vary from single counties to multicounty regions, cities, multicity regions and parts of counties. **See the lhd_area_type and lhd_note fields for more information on specific rows of data.** The municipalities included in LHDs can change over time and are reflected in the geography identifier fields.

Several states have city local health departments that run independently from the LHDs of the counties in which they are located. We subtract the relevant city populations from county LHD populations in those cases.

#### State-Specific LHD Notes

Florida: For Florida LHDs, we used population served as provided by the Florida Department of Health. For all other states, we computed the population served for each LHD by year using the Census Bureau’s intercensal [population estimates](https://www.census.gov/programs-surveys/popest.html).

Indiana: Local health department data was self-reported in a state-run survey. Some of the reported values appear to be typos, particularly in 2015 expenditures values that are many times higher or lower than the following years. Several also have data entry inconsistencies in 2015 staffing data. In those cases we made the FTE value N/A. Many departments did not fill out the survey in its entirety and have missing values for staffing and/or expenditures. State totals are therefore not provided for Indiana. Full-time equivalent staffing was not directly reported as in other states, but is calculated as full-time staff + (0.5 * part time staff).

Missouri: The cities of Joplin, Independence and Kansas City have or had independent LHDs that are not served by their local county health departments and can cross county boundaries. We used [Geocorr](http://mcdc.missouri.edu/applications/geocorr2014.html) to determine the percentage of each city’s population residing in each county in the 2010 Census, and then multiplied by population for each year in the LHD dataset. We subtracted that population from the county population to compute population served for the relevant county health departments that do not serve the cities.

Minnesota: Data from 2011 to 2018 is reported at the community health board level, while data from 2005 to 2010 is reported by local health departments. The units are the same in many areas, particularly for single-county health departments. The statewide totals are also comparable.

Ohio: Several LHDs in Ohio disbanded or merged in the mid- to late 2010s, which is reflected in this data. These changes occurred in large part because the state required LHDs to be accredited by 2020, which was difficult or impossible for small departments to achieve. **Take particular care to note the counties, cities or towns included in each department by year for any comparison over time.** Data for the newly formed Marietta-Belpre Health Department in 2017 was reported separately by city for expenditures and jointly for staffing.

#### LHD State Data Sources

Florida: [Florida Department of Health, Division of Public Health Statistics and Performance Management](http://www.flhealthcharts.com/charts/default.aspx)

Indiana: Indiana State Department of Health

Kentucky: Kentucky Cabinet for Health and Family Services

Minnesota: [Minnesota Department of Health](https://www.health.state.mn.us/communities/practice/lphact/annualreporting/archive.html)

Missouri: Missouri Department of Health and Senior Services

North Carolina: [North Carolina Department of Health and Human Services](https://schs.dph.ncdhhs.gov/data/county.cfm)

Ohio: Ohio Department of Health

Washington: [Washington Department of Health](https://www.doh.wa.gov/ForPublicHealthandHealthcareProviders/PublicHealthSystemResourcesandServices/Funding/BARS/2018RevenueReport), [The Public Health Activities and Services Tracking (PHAST) team at the University of Washington School of Nursing](https://phastdata.org/)

### State Directory (dataset 6)

The state directory dataset contains overview information on each state’s public health system.

We calculated 2016-18 annual average state spending on public health using the [State Health Expenditure Dataset](http://systemsforaction.org/projects/optimizing-governmental-health-and-social-spending-interactions/tools/state-health-expenditure-dataset-shed-2000-2013) (SHED). SHED encodes data from the Census Bureau’s [Annual Survey of State Government Finances](https://www.census.gov/programs-surveys/state.html), separating out public health expenditures. The data includes spending by all agencies and transfers to local governments. California does not submit detailed data and therefore is not included in SHED.

To calculate the 2016-18 annual averages, we inflation-adjusted public health expenditures and total expenditures from each state to 2019 dollars. We used a simple weighted average, dividing the sum of public health expenditures by the sum of population for per capita average, and the sum of public health expenditures by the sum of total expenditures for percent spent on public health. Data for Alaska was not available for 2016 or 2017, so its figures represent only 2018.

The data on governance relationship between each state and its local health departments is from the [Association of State and Territorial Health Officials](https://www.astho.org/) (ASTHO). Read more about how it defines the categories in ASTHO’s [2016 Profile Report](https://www.astho.org/Profile/Volume-Four/2016-ASTHO-Profile-of-State-and-Territorial-Public-Health/).

## Attribution

Findings and the data should be cited as: “According to a KHN and Associated Press analysis.” If you are using a specific dataset in your story, please also credit the organizations that have provided it:

National data (dataset 1) is from the [Association of State and Territorial Health Officials](https://www.astho.org/).

Dataset 2 is from the [U.S. Census Bureau Annual Survey of State and Local Government Finances](https://www.census.gov/programs-surveys/gov-finances/data/datasets.html).

Dataset 3 is from the [State Health Expenditure Dataset](http://systemsforaction.org/projects/optimizing-governmental-health-and-social-spending-interactions/tools/state-health-expenditure-dataset-shed-2000-2013) team and the [U.S. Census Bureau Annual Survey of State and Local Government Finances](https://www.census.gov/programs-surveys/gov-finances/data/datasets.html).

Datasets 4 and 5 are from state health departments; see [above](#lhd-state-data-sources) for source(s) by state

Spending on public health data by state (in dataset 6) is from the [State Health Expenditure Dataset](http://systemsforaction.org/projects/optimizing-governmental-health-and-social-spending-interactions/tools/state-health-expenditure-dataset-shed-2000-2013) and the [U.S. Census Bureau Annual Survey of State Government Finances](https://www.census.gov/programs-surveys/state.html).

## Potential Errors

This data is largely self-reported by government agencies through surveys or other mechanisms; some contain typos or mistakes. We cannot guarantee that the data is error-free, only that it is what agencies reported.

Please open a Github issue if you spot issues in your local data that are not due to this self-reporting.

## How to Contribute

We requested LHD data from many but not all states. If you have LHD-level total expenditures and/or FTE staffing data that is not included here, please reach out via Github issue.