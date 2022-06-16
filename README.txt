The files in this github are the data a scripts necessary for all results in "The challenge of life history
traits - a small cladoceran, Ceriodaphnia rigaudi" Community Ecology. 2022
Authors: Jo A. Werba and Jurek Kolasa
Corresponding author: Jo A. Werba jo.werba@gmail.com


Data Files:

cerio_pop.csv -- Ceriodaphnia riguadi population data from lab experiments
Ceriodaphnia_Feeding_Nov07_2017.csv -- Ceriodaphnia riguadi feeding raw data from experiments
ceriodaphnia_literature.csv -- complete literature search
lit_data.csv -- complete literature data
Lit_Life_History.csv -- just data from 5 papers that had life history information
pool_measures.csv -- cleaned Jamaican rock pool data

R scripts:
basic_cerio_pop_curves.R - fits population growth curves using glmm; requires cerio_pop.csv
cerio_fit_pop.R - fits population growth curves using stan; requires cerio_pop.csv, cerio_pop.stan
cerio_param_fit.R - fits R and K estimates; require cerio_pop.csv
feeding.R -- fits feeding rates; requires Ceriodaphnia_Feeding_Nov07_2017.csv
feeding_and_excretion.R -- fit feeding rate using bayesion stan model; require fec_linear_wideprior.stan, Ceriodaphnia_Feeding_Nov07_2017.csv
Graphing_Set_Up.R - graphing aesthetics
jamaica_env.R  -- runs the hurdle model for Jamaican rock pool environmental data; needs pool_measures.csv
map.R -- creates map of locations found in literature that have C. riguadi; needs lit_data.csv
transfer_functions.R -- list of possible transfer functions

stan models:
cerio_pop.stan -- model for estimating population growth
fec_linear_wideprior.stan -- model for linear feeding rate
fec_exc_wide.stan -- model for excretion rate

