### Absorption <a id="model-parameters-and-assumptions-absorption"></a>

Absorption of dabigatran etexilate is influenced by intestinal permeability and Pgp transport. The calculated value was used for `Specific intestinal permeability`. The value for Pgp kcat was estimated, informed by Rifampicin-Dabigatran Pgp-induction DDI data. 

The dissolution of capsules was implemented via an empirical Weibull function, using the Weibull parameters from the original model by [Moj et al. 2019](#main-references). 

### Distribution <a id="model-parameters-and-assumptions-distribution"></a>

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `PK-Sim Standard` for all three compounds. 
For the model parameter `Specific organ permeability` the calculated values were used for all three compounds, with the `Lipophilicity` values optimized to best match clinical data (see [Section 2.3.4](#model-parameters-and-assumptions-absorption)). 

### Metabolism and Elimination <a id="model-parameters-and-assumptions-metabolism-and-elimination"></a>

- For dabigatran etexilate the final model includes transport by Pgp, prodrug ester cleavage by CES1 and CES2 and passive renal filtration (trace amounts excreted in urine following oral administration). 
- For dabigatran the final model includes glucuronidation by UGT2B15 and renal excretion (70.6-76.2% excreted in urine following intravenous, 4.3% excreted in urine following oral administration). 
- For dabigatran glucuronide the final model includes renal excretion only, implemented with the GFR fraction parameter value from the original model by [Moj et al. 2019](#main-references). Dabigatran glucuronide in urine is not meaningful in clinical practice (2.7-6.4% excreted in urine following intravenous, 0.4% excreted in urine following oral administration) and there is little data to inform the estimation of dabigatran glucuronide GFR fraction. 

### Automated Parameter Identification <a id="model-parameters-and-assumptions-parameter-identification"></a>

These are the results of the two final sequential parameter identifications.
1. iv: 

| Model Parameter      | Optimized Value | Unit |
| -------------------- | --------------- | ---- |
| `Dabigatran logP` | 1.1436481967                |      |
| `Dabigatran UGT2B15 kcat` | 4.2993761606                | 1/min     |
| `Dabigatran GFR fraction` | 1.2278243749                |      |
| `Dabigatran glucuronide logP` | -0.80                |      |
| `Dabigatran glucuronide GFR fraction` | 6.36 (fixed)                |      |

2. oral: 

| Model Parameter      | Optimized Value | Unit |
| -------------------- | --------------- | ---- |
| `Dabigatran etexilate logP` | 1.8088312812                |      |
| `Dabigatran etexilate Pgp kcat` | 0.46                | 1/min     |
| `Dabigatran etexilate CES1 kcat` | 10.8149677921                | 1/min     |
| `Dabigatran etexilate CES2 kcat` | 0.7209978528                | 1/min     |
| `Dabigatran etexilate GFR fraction` | 1.00 (fixed)                |      |
