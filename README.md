# Project-02 - Classification

## Overview
As a potential investor or hire, how can you assess whether to further invest or join a startup? This project will predict type of exit (acquisition, IPO, shutdown) for a startup given current funding and company information.
This can help potential investors or employees to look out factors to assess a startup and the potential exit path.

## Data Source
[Crunchbase 2013 Snapshot © 2013](https://data.crunchbase.com/docs/2013-snapshot)
* Data set for ~ 50,000 companies

## Features
| Feature                       | Type                   |
|-------------------------------|------------------------|
| # Employees                   | Numerical              |
| # Founders                    | Numerical              |
| Last Funding Round            | Ordinal (e.g. A, B, C) |
| HQ Region                     | Categorical            |
| # Funding Rounds              | Numerical              |
| # Total Funding               | Numerical              |
| Years Active                  | Numerical              |
| Largest Funding Round To-Date | Numerical              |
| Avg # days between Rounds     | Numerical              |
| Market sector                 | Categorical            |

## Potential Challenges
* The initial data is in mysql, and will need to migrate to the required postgress sql for analysis with a tool that does not result in data fidelity issues during migration
* There is some data cleaning needed to filter out companies with the predictor value to include in training set
* There is also initial data engineering needed to generate the desired features from the raw data set
* If the initial proposed features are not good predictors, more time maybe needed to research what makes better predictor features
