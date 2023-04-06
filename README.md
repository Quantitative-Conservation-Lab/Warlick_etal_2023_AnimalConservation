## *Demographic and environmental drivers of population dynamics and viability in an endangered top predator using an integrated model* 

#### Amanda J. Warlick, Gina K. Himes Boor, Tamara L. McGuire, Kim E.W. Shelden, Eiren K. Jacobson, Charlotte Boyd, Paul R. Wade, André E. Punt, Sarah J. Converse

##### Please contact the first author for questions about the code or data: Amanda Warlick (amandajwarlick@gmail.com)

##### Secondary contact: Sarah Converse (sconver@usgs.gov)

______________________________________________________________________________________

## Abstract

Knowledge about the demographic and environmental factors underlying population dynamics is fundamental to designing effective conservation measures to recover depleted wildlife populations. However, sparse monitoring data or persistent knowledge gaps about threats make it difficult to identify the drivers of population dynamics. In situations where small, declining, or depleted populations show continued evidence of decline for unknown reasons, integrated population models can make efficient use of available data to improve our understanding of demography, provide fundamental insights into factors that may be limiting recovery, and support conservation decisions. We used mark-resight and aerial survey data from 2004-2018 to build an integrated population model for the Cook Inlet population of beluga whales (*Delphinapterus leucas*), which is listed as endangered under the U.S. Endangered Species Act. We examined the effects of prey availability and oceanographic conditions on beluga vital rates and conducted a population viability analysis to predict extinction risk across a range of hypothetical changes in beluga survival and reproduction. Our results indicated that while survival of breeding females (0.97; 95% CI 0.95-0.99) and young calves (0.92; 0.80-0.98) was relatively high, survival of non-breeders (0.94; 0.91-0.97) and fecundity (0.28; 0.22-0.36) may be depressed. Furthermore, our analysis indicates that the population will likely continue to decline, with a 17-32% probability of extinction in 150 years. Our model highlights the utility of integrated population modeling for maximizing the usefulness of available data and identifying factors contributing to the failure of protected populations to recover. This framework can be used to evaluate proposed conservation and recovery efforts for this and other endangered species. 

### Table of Contents 

#### [Scripts](./scripts)

Contains the script to run all analyses: CIBW_ME_IPM_PVA.Rmd.
 
#### [Data](./Data) 

Contains raw and processed data necessary for running the model, including mark-resight data and oceanographic and prey-related covariate data. 

#### [Results](./results)

Contains raw and processed results.  

#### Required Packages and Versions Used 

Hmisc_4.5-0       
ggstance_0.3.5   
reshape2_1.4.4    
truncnorm_1.0-8   
DescTools_0.99.43 c
cowplot_1.1.1     
demogR_0.6.0     
gtools_3.9.2
knitr_1.31        
stringr_1.4.0    
purrr_0.3.4       
ggplot2_3.3.6     
tidyverse_1.3.1   
dplyr_1.0.5      
readr_2.0.1       
here_1.0.1        
tidyr_1.1.3       
lubridate_1.7.10 

#### Details of Article 

Warlick, AJ, Himes Boor, GK, McGuire, TL, Shelden, KEW, Jacobson, EK, Boyd, C, Wade, PR, Punt, AE, Converse, SJ. 2023. Demographic and environmental drivers of population dynamics and viability in an endangered top predator using an integrated model. *Animal Conservation*.

#### How to Use this Repository 

The CIBW_ME_IPM_PVA.Rmd markdown file is not designed to knit but includes code chunks that users can use to:   
- Load mark-resight, aerial survey, and covariate data (user must select whether seasonal or annual covariates are desired)  
- Run null, random effects models, or covariate models  
-- Code is available to run models in both jags and NIMBLE, the latter of which were used to conduct the posterior predictive check and WAIC values  
- Examine model results  
- Run population viability analyses (PVA) population projections and calculate extinction risk metrics   
- Calculate population sensitivity correlations  
- Run population projections across changes in demographic rates  
- Examine code used to assess model results and population projections displayed in appendices, including ages at first reproduction, aerial survey detection prior and aerial survey source data, and the development of a quasi-extinction level  

