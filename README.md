
# UNICEF-WHO-World Bank Joint Child Malnutrition Estimates Stunting and Overweight Global Health Estimates (2025 Edition)

This GitHub repository contains code and sample data for models used by UNICEF, WHO and the World Bank to generate global health estimates for stunting and overweight. 
These estimates are published biennially as the UNICEF-WHO-World Bank Joint Malnutrition Estimates. 

https://data.unicef.org/resources/jme

www.who.int/teams/nutrition-and-food-safety/monitoring-nutritional-status-and-food-safety-and-events/joint-child-malnutrition-estimates

https://datatopics.worldbank.org/child-malnutrition/

## Updates to Modeling Approach Since 2023 Edition


## Model
The model used in these analyses is similar to that proposed in McLain et al. (2019) [^1]   The general statistical model is a penalized longitudinal mixed model with a heterogeneous error term. The non-linear longitudinal patterns in the outcomes were captured using penalized cubic B-splines, with country-specific intercepts and random cubic B-splines. 

## Procedure for Generating Stunting and Overweight Modelled Estimates

### Contents
1. Preparing Covariates

2. Preparing Primary Data

3. Model

4. Results

Additional Folders

- **Data**: Contains survey prevalence estimates, raw covariate data,
  country-level classifications, and outputted analysis files.
- **Figures**: Contains outputted figures displaying the results.
- **Utils**: Contains various programs and functions required to run the
  analyses.

### Set-up

All the programs in the folders `Preparing Primary Data`, `Model`, and
`Results` need to be run separately for both Stunting and Overweight.
Ensure that you read each file carefully to verify that the files are
named and stored correctly.

## References

For further reading on the technical details and applications, please
refer to the McLain et al. (2019).

## License

This project is licensed under the MIT License. See the LICENSE file for
details.

## Contact

For questions or issues, please contact the repository maintainer.

## Acknowledgments

### Code
We thank Alexander McLain (@alexmclain) for the development and implementation of the model code.

### Conceptualization of the Model
We thank Alexander McLain, Edward Frongillo, Monika Blössner, Juan Feng, Elaine Borghi, Chika Hayashi, Julia Krasevec, Gretchen Stevens, Mariel Finucane, Leontine Alkema and Simon Cousens, Nicholas Kassebaum for their helpful comments and contributions to this project. 

### Input Data
#### Joint Malnutrition Estimates 2023 Edition
UNICEF: 

WHO: 

World Bank Group: 

#### Covariates
Global Burden of Disease Collaborative Network Institute for Health Metrics and Evaluation (IHME)

## References

[^1]: •	McLain A.C., E.A. Frongillo, E. Borghi, and J. Feng (2019). Prediction intervals for heterogeneous penalized longitudinal models with multi-source summary measures: an application to estimating child malnutrition rates. Statistics in Medicine 38:1 1002–1012. GitHub Repo: https://github.com/alexmclain/PHMM
