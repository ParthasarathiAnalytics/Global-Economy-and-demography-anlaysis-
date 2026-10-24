# Global Economy and Demographic Analysis 🌍

**A data analytics project exploring global population, GDP, demographic
indicators, and regional economic patterns using Excel, SQL, and Power
BI.**

**Author:** Parthasarathi A\
**Project Repository:** `Global-Economy-and-demography-anlaysis-`

------------------------------------------------------------------------

## 📌 Project Overview

This project combines country-level demographic and economic data to
explore how population, GDP, literacy, infant mortality, land area,
coastline, birth and death rates, and sector contributions vary across
countries and regions.

The project uses multiple data sources and tools: - **SQL** to define
and query a country-level dataset. - **Excel** to work with historical
GDP and supporting datasets. - **Power BI** to present findings through
an interactive dashboard. - **CSV and Excel files** to store
demographic, country metadata, population, and GDP data.

The supplied Power BI report is `LAST TRY.pbix`. The supporting project
files include `CountriesWorld.sql`, `GDP by country 1960-2016.xlsx`,
`MetaData Country.csv`, and `PopulationPerCountry.csv`.

## 🎯 Project Objectives

-   Compare population and economic indicators across countries.
-   Explore GDP patterns over time, including the 1960--2016 period in
    the supplied GDP workbook.
-   Compare demographic indicators such as literacy, infant mortality,
    birth rate, death rate, and net migration.
-   Examine country and regional differences in agriculture, industry,
    and services.
-   Explore land area, population density, coastline ratio, and GDP
    relative to land area.
-   Present key comparisons and observations in a Power BI report.
-   Translate the analysis into findings that can support further
    economic and demographic investigation.

## 🧩 Business Problem

Economic and demographic indicators are spread across different datasets
and can be difficult to compare consistently. Analysts need a structured
way to bring these data together, inspect country-level differences, and
communicate regional patterns.

This project organizes country metadata, population information,
historical GDP values, and country indicators to support comparative
analysis through SQL, Excel, and Power BI.

## 🛠️ Tools and Technologies

  -----------------------------------------------------------------------
  Tool / Technology                   Role in the project
  ----------------------------------- -----------------------------------
  **Microsoft Excel**                 Inspect and prepare tabular data,
                                      including historical GDP

  **SQL**                             Create a database and country-level
                                      table; support structured querying

  **Power BI**                        Build and view the interactive
                                      report (`LAST TRY.pbix`)

  **CSV**                             Store population and country
                                      metadata

  **XLSX**                            Store GDP by country and year

  **DAX / Power Query**               Power BI modelling and
                                      transformations, where used in the
                                      report
  -----------------------------------------------------------------------

> The supplied files confirm the use of Excel, SQL, and Power BI.
> Specific DAX measures, Power Query transformations, and report
> interactions should be documented from the actual PBIX if a detailed
> technical inventory is needed.

## 📂 Project Files

  -----------------------------------------------------------------------
  File                                Description
  ----------------------------------- -----------------------------------
  `CountriesWorld.sql`                SQL script that creates the
                                      `countries` database and
                                      `countries_world` table, then
                                      inserts country-level indicators

  `GDP by country 1960-2016.xlsx`     Historical GDP workbook with sheets
                                      for GDP by country; the main sheet
                                      covers 1960--2016

  `MetaData Country.csv`              Country code, region, income group,
                                      special notes, and country name

  `PopulationPerCountry.csv`          Population / World Development
                                      Indicators source export

  `LAST TRY.pbix`                     Power BI report file

  `FINDING AND INSIGHTS(1).docx`      Project notes describing reported
                                      findings and interpretations
  -----------------------------------------------------------------------

## 🗃️ Data Overview

### 1. Country indicators --- SQL

The `countries_world` table contains fields including:

-   `Country`, `Country_Code`, `Region`
-   `Population`, `Area_sq_mi`, `Pop_Density`
-   `Coastline_Ratio`, `Net_Migration`
-   `Infant_Mortality`, `GDP_per_Capita`, `Literacy`
-   `Phones_per_1000`, `Arable_Percent`, `Other_Percent`, `Climate`
-   `Birthrate`, `Deathrate`
-   `Agriculture`, `Industry`, `Service`

### 2. Country metadata --- CSV

`MetaData Country.csv` includes:

-   Country Code
-   Region
-   IncomeGroup
-   SpecialNotes
-   Country

This file can support country lookups and region- or income-group
comparisons.

### 3. GDP by country --- Excel

The GDP workbook includes country name and code, indicator name and
code, and year columns. The main sheet is named
`GDP BY COUNTRY 1960-2016` and covers annual values from 1960 through
2016.

### 4. Population --- CSV

`PopulationPerCountry.csv` is an export labelled **World Development
Indicators**. It includes metadata/header rows before the country data,
so inspect and clean the file before using it for analysis.

## 🔄 Suggested Analysis Workflow

1.  Inspect each file and identify its grain, columns, units, and date
    coverage.
2.  Clean country names, country codes, data types, missing values, and
    malformed values.
3.  Use country codes where possible to match country metadata to the
    indicator tables.
4.  Import the country-level SQL data and run queries for comparisons
    and summaries.
5.  Prepare the GDP and population files in Excel or Power Query.
6.  Model the data in Power BI, using relationships between country
    codes and other appropriate keys.
7.  Create report visuals for country comparisons, regional summaries,
    and historical GDP trends.
8.  Validate the results against the source data and document the key
    findings.
9.  Publish or share the Power BI report with the cleaned data and this
    README.

## 📈 Analysis Areas

The project notes cover the following analysis areas:

-   **Population:** compare population levels by country.
-   **GDP:** compare economic output across countries and regions.
-   **Infant mortality:** examine differences in reported infant
    mortality indicators.
-   **Literacy:** compare literacy rates across countries.
-   **Growth trends:** examine birth rates, death rates, natural growth,
    and regional sector patterns.
-   **Economic sectors:** compare agriculture, industry, and services.
-   **Land area and population density:** explore country size and
    population concentration.
-   **Coastline ratio:** compare coastline-related indicators.
-   **GDP relative to area:** explore GDP per unit of land area, where
    the required measures and units are available.
-   **Income groups and regions:** compare country indicators by
    metadata categories.

## 🔍 Findings Recorded in the Project Notes

The supplied `FINDING AND INSIGHTS(1).docx` records these observations:

-   China is identified in the notes as the highest-population country,
    with a population described as nearly one billion. British Virgin
    Islands and Cayman Islands are listed among the lowest-population
    entries.
-   The notes identify Luxembourg as having the highest GDP and list
    Western Sahara and Somalia among the lowest GDP entries.
-   Burkina Faso and Niger are listed among countries with lower
    literacy rates; Bosnia and Herzegovina is listed as having a high
    literacy rate.
-   Latin America is described in the notes as performing strongly
    across agriculture, industry, and services, while Northern Africa is
    described less favorably in those sectors.
-   European countries are described as representing the high-income
    category, while African countries are associated with the low-income
    category.
-   Russia, Canada, and the United States are listed among countries
    with large land areas.
-   The notes identify Baltic and Eastern Europe as regions with
    relatively balanced birth and death rates.
-   Albania, Réunion, and the Marshall Islands are listed as having high
    coastline-related values.
-   Monaco, Macau, and Hong Kong are listed among countries with high
    GDP relative to area.

### Important validation note

These are **observations transcribed from the supplied project notes**,
not independently revalidated conclusions. Some figures or labels in the
notes appear inconsistent with the named indicators or units---for
example, several values resemble malformed or misformatted data. Verify
the original source rows, units, calculations, and Power BI visuals
before presenting these statements as final quantitative results. Do not
treat the recorded rankings as confirmed until validation is complete.

## 💼 Potential Business Value

When the underlying data has been validated, this type of analysis can
help users:

-   Compare country-level economic and demographic profiles.
-   Identify regional differences in population and development
    indicators.
-   Review historical GDP patterns across countries.
-   Segment countries by region and income group.
-   Communicate patterns through a consolidated Power BI report.
-   Identify data quality issues that need attention before
    decision-making.

## ▶️ How to Use the Project

### SQL

1.  Open `CountriesWorld.sql` in a compatible SQL environment, such as
    MySQL Workbench.
2.  Review the script before execution: it contains
    `DROP DATABASE IF EXISTS countries`, which deletes an existing
    database with that name.
3.  Run the script only in a suitable development environment after
    backing up any database that must be preserved.
4.  Query the resulting `countries_world` table to explore country
    indicators.

Example query after the database has been created:

``` sql
USE countries;

SELECT
    Country,
    Region,
    Population,
    GDP_per_Capita,
    Literacy
FROM countries_world
ORDER BY Population DESC;
```

### Excel

1.  Open `GDP by country 1960-2016.xlsx`.
2.  Use the `GDP BY COUNTRY 1960-2016` sheet for the 1960--2016 annual
    series.
3.  Inspect blanks, zeros, country codes, and year columns before
    drawing conclusions.
4.  Use country codes to support reliable matching with metadata.

### Power BI

1.  Open `LAST TRY.pbix` in Microsoft Power BI Desktop.
2.  Review the model, relationships, transformations, measures, and
    report pages.
3.  If the report requests local source files, reconnect them to the
    appropriate files in this repository.
4.  Refresh the data and verify key totals, rankings, labels, and units
    before sharing.

## 📁 Suggested Repository Structure

``` text
Global-Economy-and-demography-anlaysis-/
├── README.md
├── CountriesWorld.sql
├── GDP by country 1960-2016.xlsx
├── MetaData Country.csv
├── PopulationPerCountry.csv
├── LAST TRY.pbix
└── FINDING AND INSIGHTS.docx
```

The structure above reflects the files supplied for documentation.
Adjust filenames if the actual GitHub repository uses different names.

## 🚀 Future Improvements

-   Document the exact data sources, publication dates, and indicator
    definitions.
-   Standardize country codes and validate joins across all datasets.
-   Correct malformed values and define explicit missing-value rules.
-   Record the exact units for GDP, infant mortality, coastline ratio,
    and GDP per area.
-   Add a data dictionary and a reproducible cleaning workflow.
-   Document Power BI pages, KPIs, DAX measures, and model
    relationships.
-   Add screenshots of the report pages to the README.
-   Recalculate the findings from validated data and include exact
    values and time periods.

## 👤 Author

**Parthasarathi A**

-   GitHub:
    [ParthasarathiAnalytics](https://github.com/ParthasarathiAnalytics)
-   Portfolio:
    [parthasarathi-analytics.vercel.app](https://parthasarathi-analytics.vercel.app/)

------------------------------------------------------------------------

*This README is based on the project files and findings document
supplied for this repository. Findings that have not been recalculated
from validated source data are explicitly identified as project-note
observations.*
