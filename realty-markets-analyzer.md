# Realty Market Analyzer

## Overview

This is a project idea to gather data and develop an analysis of realty markets across the US for the purpose of long term investment properties. There are two major types of investment:

- investment for appreciation
- investment as a rental property

There are many housing price and appreciation prediction tools, but there isn't many (any?) that effectively assess factors to assist with the second type of investment: rental properties.

This project seeks to address that gap.

## Table of Contents

* [Background](#background)
* [Data Sources](#data-sources)
* [EDA and visualization](#EDA-and-visualization)
* [Project Plan](#project-plan)
* [MVP (minimum viable product)](#mvp-minimum-viable-product)
* [Future plans](#future-plans)

## Background

The concept of buying property with the intention to rent comes down to some simple math for now.  You need to be able to the pay the mortgage and all expenses with the rental income to enable positive cash flow as well as building equity from day 1.  A common rule is the "1 % rule", [best explained here](https://affordanything.com/one-percent-rule-gross-rent-multiplier/).  In essence, it is similar to a price to earnings ratio in the stock market as a filter - you want the monthly rent to be at least 1% of the purchase price.  This leads to payoff in about 8 years.  This section will be further built out and developed later.
An example of a company in this space is: 
[Attomdata](https://www.attomdata.com/industries/real-estate).

## Data sources

I am dividing this into two sections in case I am not able to integrate all data initially.

Essential data:

| Data                | Source                              | Purpose    | Details
| :----------------   | :---                                | :---       | :---
| House prices and rent prices      | [Zillow](https://www.zillow.com/research/data/) | with rent prices, can determine ratios | TBA
| New construction                  | [Census data](https://www.census.gov/construction/nrc/index.html) | While prices are lagging indicator, this should be a leading indicator | only high level data :( maybe this is better: [Census surveys](https://www.census.gov/construction/bps/msaannual.html)
| Rental Vacancy rates (Table 4)     | [more Census](https://www.census.gov/housing/hvs/data/rates.html) | could be a proxy for rent prices which is hard to find | this is 75 largest metro areas
| sub-county population estimates    | [Census pop data](https://www.census.gov/data/tables/time-series/demo/popest/2010s-total-cities-and-towns.html#ds)   | population trends will indicate future rent demand | TBA

Data that will be useful for modeling down the road as additional factors:

* Population:
https://www.census.gov/data/developers/data-sets/popest-popproj.html

* BLS unemployment:
https://download.bls.gov/pub/time.series/la/

* Economic indicators:
https://www.census.gov/programs-surveys/susb/data/tables.html

* Additional information on rent prices:
https://www.huduser.gov/portal/datasets/fmr.html

* Crime etc other factors:
https://www.huduser.gov/portal/datasets/socds.html

* Foreclosure data?

## EDA and visualization
Because time series data will be complicated to analyze, I will focus initially on looking across the US at one timepoint: June 2019.  If I have time, I will look at June 2020 but COVID-19 may really affect 2020 data.  Ideally, I will focus on time points that I will be able to find detailed rent data as potential training data and to test the accuracy of any modeling approaches.

On initial inspection, this data should lend itself nicely to these types of EDA, comparisons, and visualization.  

* Binning data by markets or geographical regions (some simple means, box plots, bar plots etc)
* looking at variation and Standard Deviation and distribution of data (histograms, etc)
* Using ANOVA to test if regions are really different than eachother
* Building choropleth maps of the data.

## Project plan
The initial plan for the week of July 20 - July 24 is:

| Date                | Goal                                | Details
| :----------------   | :---                                | :---
| Monday July 20      | Organize and merge data into SQL db | details TBA
| Tuesday July 21     | Summary data and initial EDA        | details TBA
| Wednesday July 21   | create plots and maps               | details TBA
| Thursday July 21    | EDA and testing                     | if time, build folio/flask app for maps
| Friday July 21      | Presentation                        | if time, finish any presentation material, possibly put together some github io slides

## MVP (minimum viable product)

For the initial week ending July 24, the MVP is:

1. Data organized in a database and 3 plots and 1 hypothesis test (I would love to do some Bayesian since I have never done this with real data - can we talk about this?)
2. above, plus more plots and a choropleth
3. above, plus a nicer presentation format and maps hosted online in a flask / docker app

## End User and applications

The intended end users and market will be those looking to invest in realty with data supported decision making tools.  Ideally this will be in a subscription website or app format.

## Risk management

Initially this is addressed under the MVP section but this will be updated as the project proceeds.

## Skills

I would like to highlight the following skills with this project:

* API use
* SQL, pandas
* plotting in matplotlib
* Bayesian??
* Docker, AWS, flask, folio

## Future plans
* do it!