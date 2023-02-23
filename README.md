# WHO_COVID_19_Global_Vaccinations

## Personal Data Analysis Portfolio Project

### Purpose:
The purpose of this Jupyter Notebook is to show my thinking when analyzing new data. I am more familiar with data analysis in R using RStudio, but I am using Python and Pandas in PyCharm for this project for the practice, and to add to my portfolio.

### Why this data?
I looked for a simple, but interesting .csv dataset on the WHO data portal. This is historical vaccination data by Country and World Health Organization Region showing reported vaccinations by country to the last reported date.

### Source of Data:
This is a static dataset, downloaded from [The World Health Organization] (https://covid19.who.int/data) on Friday, February 17, 2023
The url to the evergreen data set is: (https://covid19.who.int/who-data/vaccination-data.csv)

### Data Fields:

**FIELD source-data-type
    source-description:**

- COUNTRY String
    - Country, territory, area
- ISO3 String
    - ISO Alpha-3 country code
- WHO_REGION String
   - WHO regional offices: WHO Member States are grouped into six WHO regions:
       - Regional Office for Africa (AFRO),
       - Regional Office for the Americas (AMRO),
       - Regional Office for South-East Asia (SEARO),
       - Regional Office for Europe (EURO),
       - Regional Office for the Eastern Mediterranean (EMRO),
       - Regional Office for the Western Pacific (WPRO).
- DATA_SOURCE String
    - Indicates data source:
        - REPORTING: Data reported by Member States, or sourced from official reports
        - OWID: Data sourced from Our World in Data: https://ourworldindata.org/covid-vaccinations
- DATE_UPDATED Date
    - Date of last update
- TOTAL_VACCINATIONS Integer
    - Cumulative total vaccine doses administered
- PERSONS_VACCINATED_1PLUS_DOSE Decimal
    - Cumulative number of persons vaccinated with at least one dose
- TOTAL_VACCINATIONS_PER100 Integer
    - Cumulative total vaccine doses administered per 100 population
- PERSONS_VACCINATED_1PLUS_DOSE_PER100 Decimal
    - Cumulative persons vaccinated with at least one dose per 100 population
- PERSONS_FULLY_VACCINATED Integer
    - Cumulative number of persons fully vaccinated
- PERSONS_FULLY_VACCINATED_PER100 Decimal
    - Cumulative number of persons fully vaccinated per 100 population
- VACCINES_USED String
    - Combined short name of vaccine: “Company - Product name” (see below)
        * I will be tidying the data to split this field into company and product, and making a separate table pivoted longer by Country
- FIRST_VACCINE_DATE Date
    - Date of first vaccinations. Equivalent to start/launch date of the first vaccine administered in a country.
- NUMBER_VACCINES_TYPES_USED Integer
    - Number of vaccine types used per country, territory, area
- PERSONS_BOOSTER_ADD_DOSE Integer
    - Persons received booster or additional dose
- PERSONS_BOOSTER_ADD_DOSE_PER100 Decimal
    - Persons received booster or additional dose per 100 population
