# sg-income-poverty-estimates
## Income And Poverty Modelled Estimates
This dataset includes information about estimated Edinburgh household income, and percent of Edinburgh households with low incomes.

These indicators were produced as part of the Income Modelling Project, carried out by Heriot-Watt University, which aimed to develop improved measures of local incomes and poverty in Scotland at small area level. The project was commissioned at the end of 2011 by the Improvement Service working on behalf of City of Edinburgh, Falkirk, Fife and Highland Councils and the Scottish Government. Modelled estimates are provided for (nearly) every data zone in Scotland. For further information about the project and to access the full publication, please visit the Income Modelling Project webpage at: http://www.improvementservice.org.uk/income-modelling-project

Median income measures the income which 50% of households have less than, and 50% more than. Gross income covers income from all sources (wages, salaries, pensions, benefits, rent, interest, maintenance) before the deduction of tax and national insurance contributions.

Material deprivation covers households lacking several items, which are regarded as essentials of life in Britain today by a majority of the population, because they cannot afford them.

First Benefit Unit (FBU) covers the core household unit comprising householder, partner and dependent children, which would be treated as a single income unit by the UK Benefits system; this excludes grown-up children and other adult members of household.

Low income poverty is having less than 60% of the national median income, using net equivalised income either before or after housing costs; this is sometimes referred to as relative poverty.

Modelled estimates are available for (nearly) every datazone in Scotland. Estimates of precision should be considered when making comparisons across areas (see Annex E from the 'Local Incomes and Poverty in Scotland' report, March 2013).


Statistics provided by Scottish Government:  http://statistics.gov.scot/data/income-and-poverty-modelled-estimates

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/sg-income-poverty-estimates.git
```

Install npm dependencies

```
cd sg-income-poverty-estimates
npm install
```

Run the API (from the sg-income-poverty-estimates directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
