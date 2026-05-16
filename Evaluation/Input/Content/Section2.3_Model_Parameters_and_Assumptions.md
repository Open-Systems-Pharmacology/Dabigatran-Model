### Absorption <a id="model-parameters-and-assumptions-absorption"></a>

For the model parameters `Specific intestinal permeability` and `Specific organ permeability` calculated values were used for all three compounds. Instead, the `Lipophilicity` values were optimized to best match clinical data (see [Section 2.3.4](#model-parameters-and-assumptions-parameter-identification)). Parameter optimizations of logP values (iv first, then oral) were informed by clinical dabigatran etexilate, dabigatran and total dabigatran (sum of dabigatran + dabigatran glucuronide) plasma concentration data. Parameter optimization of the Pgp kcat value was informed by addition of the Rifampicin-Dabigatran Pgp-induction DDI trial data. 

The dissolution of capsules was implemented via an empirical Weibull function using the Weibull parameters from the original model by [Moj et al. 2019](#main-references). 

### Distribution <a id="model-parameters-and-assumptions-distribution"></a>

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `PK-Sim Standard` for all three compounds. 
`Lipophilicity` values were optimized to best match clinical data (see [Section 2.3.1](#model-parameters-and-assumptions-absorption)); for `Specific organ permeability` the calculated values were used for all three compounds. 

### Metabolism and Elimination <a id="model-parameters-and-assumptions-metabolism-and-elimination"></a>

... 
For dabigatran glucuronide GFR fraction, the parameter values from the original model by [Moj et al. 2019](#main-references) was kept, as dabigatran glucuronide in urine is not meaningful in clinical pratice (2.7-6.4% excreted in urine following intravenous, 0.4% excreted in urine following oral administration) and we had very little data to inform its estimation. 

### Automated Parameter Identification <a id="model-parameters-and-assumptions-parameter-identification"></a>

This is the result of the final parameter identification.

| Model Parameter      | Optimized Value | Unit |
| -------------------- | --------------- | ---- |
| `PK-Sim parameter 1` |                 |      |
| `PK-Sim parameter 2` |                 |      |
| `PK-Sim parameter 3` |                 |      |
| `PK-Sim parameter 4` |                 |      |

