# Self-reported life satisfaction vs. GDP per capita - Data package

This data package contains the data that powers the chart ["Self-reported life satisfaction vs. GDP per capita"](https://ourworldindata.org/grapher/gdp-vs-happiness?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website.

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The remaining columns are the data columns, each of which is a time series. If the CSV data is downloaded using the "full data" option, then each column corresponds to one time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data columns are transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

### How we process data at Our World In Data
All data and visualizations on Our World in Data rely on data sourced from one or several original data providers. Preparing this original data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/)

## Detailed information about each time series


## Self-reported life satisfaction
Average of survey responses. The survey question asks respondents their current position on a hypothetical [ladder](#dod:cantril-ladder), where the best possible life for them is a 10, and the worst possible life is a 0.
Last updated: March 28, 2025  
Next update: March 2026  
Date range: 2011–2024  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Wellbeing Research Centre (2025) – with major processing by Our World in Data

#### Full citation
Wellbeing Research Centre (2025) – with major processing by Our World in Data. “Self-reported life satisfaction” [dataset]. Wellbeing Research Centre, “World Happiness Report 2025” [original data].
Source: Wellbeing Research Centre (2025) – with major processing by Our World In Data

### What you should know about this data
* The Cantril ladder asks respondents to think of a ladder, with the best possible life for them being a 10 and the worst possible life being a 0. They are then asked to rate their own current lives on that 0 to 10 scale.
* The rankings are three-year averages, calculated by the World Happiness report based on nationally representative samples collected by the Gallup World Poll. The data for the 2025 report draws from survey data from 2022-2024.
* We show the data for final year of the three-year survey period, i.e. we show the 2022-2024 survey data for the year 2024.
* The number of people and countries surveyed varies year to year, but typically more than 100,000 people in 130 countries participate in the Gallup World Poll each year.
* The rankings are based entirely on the survey scores, which are weighted by Gallup to make the estimates representative.

### Source

#### Wellbeing Research Centre – World Happiness Report
Retrieved on: 2025-03-28  
Retrieved from: https://worldhappiness.report/ed/2025/  

#### Notes on our processing step for this indicator
We calculated the average of regions by taking a population-weighted average over all countries within that region.


## GDP per capita – In constant international-$ – World Bank
Average economic output per person in a country or region per year. This data is adjusted for inflation and differences in living costs between countries.
Last updated: September 8, 2025  
Next update: September 2026  
Date range: 1990–2024  
Unit: international-$ in 2021 prices  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Eurostat, OECD, IMF, and World Bank (2025) – with minor processing by Our World in Data

#### Full citation
Eurostat, OECD, IMF, and World Bank (2025) – with minor processing by Our World in Data. “GDP per capita – World Bank – In constant international-$” [dataset]. Eurostat, OECD, IMF, and World Bank, “World Development Indicators 122” [original data].
Source: Eurostat, OECD, IMF, and World Bank (2025) – with minor processing by Our World In Data

### What you should know about this data
* GDP per capita is a comprehensive measure of people's average income. It helps compare income levels across countries and track how they change over time. It is especially useful for understanding trends in economic growth and living standards.
* GDP per capita is calculated as the value of all final goods and services produced each year in a country (the [gross domestic product](#dod:gdp)), divided by the population. It represents the average economic output per person.
* This indicator shows the large inequality between people in different countries. In the poorest countries, average incomes are below $1,000 per year; in rich countries, they are more than 50 times higher.
* This data is expressed in constant international dollars to adjust for inflation and differences in living costs between countries. Read more in our article, [What are international dollars?](https://ourworldindata.org/international-dollars)
* This data comes from the World Bank and starts in 1990. For estimates going back several centuries, explore our chart of GDP per capita from the [Maddison Project Database](https://ourworldindata.org/grapher/gdp-per-capita-maddison-project-database).

### Source

#### Eurostat, OECD, IMF, and World Bank – World Development Indicators
Retrieved on: 2025-09-08  
Retrieved from: https://data.worldbank.org/indicator/NY.GDP.PCAP.PP.KD  


## World regions according to OWID
Regions defined by Our World in Data, which are used in OWID charts and maps.
Last updated: January 1, 2023  
Date range: 2023–2023  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Our World in Data – processed by Our World in Data

#### Full citation
Our World in Data – processed by Our World in Data. “World regions according to OWID” [dataset]. Our World in Data, “Regions” [original data].
Source: Our World in Data

### Source

#### Our World in Data – Regions


    