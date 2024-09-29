
# Preparing Covariates

This folder contains the code used to create the multiply imputed
datasets for the socio-demographic index (SDI) and health system access
(MCI) covariates, which were obtained from the Institute of Health
Metrics and Evaluation (IHME). SDI is a summary measure that identifies
where countries or other geographic areas sit on the spectrum of
development. Expressed on a scale of 0 to 1, SDI is a composite average
of the rankings of the incomes per capita, average educational
attainment, and fertility rates of all areas in the Global Burden of
Disease study. SDI and MCI data are missing for some countries and are
available up to 2022. Countries with missing data and values for 2023
(for all countries) are imputed 20 times.

## Data Sources

The following data sources are used and can be found in the
`Data/IHME_covs` folder:

- **GBD 2022 MCI and SDI.csv**: MCI and SDI covariate information from
  IHME.
- **API_NY.GDP.MKTP.CD_DS2_en_csv_v2_4701247.csv**: Gross Domestic Product by country and year (obtained from https://data.worldbank.org/indicator/NY.GDP.MKTP.CD). 
- **WPP2022_Demographic_Indicators_Medium.csv**: Additional demographic indicators (obtained from https://population.un.org/wpp/Download/Archive/CSV/).
- **Tidy_World_Devel_Indic.rds**: Used as an intermediate merging dataset. Not a data source.

## Imputation Process

The `Imputation of IHME covariate data_multiple_impute.R` script is
structured as follows:


## Usage

To run the imputation process, change `wd` so that the working drive
will be at the folder that contains the *“1 - Preparing Covariates”*
folder. Then execute the
`Imputation of IHME covariate data_multiple_impute.R` script. Ensure
that all data files are correctly placed in the `Data/IHME_covs` folder.

## Contact

For questions or issues regarding this folder, please contact the
repository maintainer.
