### Absorption <a id="model-parameters-and-assumptions-absorption"></a>

The model parameters `Specific intestinal permeability` and `Specific organ permeability` were set to calculated for all three compounds in the model. Instead, `Lipophilicity` was optimized to best match clinical data (see Section 2.3.4). Parameter optimizations of logP values (iv first, then oral) were informed by clinical dabigatran etexilate, dabigatran and total dabigatran (sum of dabigatran + dabigatran glucuronide) plasma concentration data. Parameter optimization of Pgp kcat value was informed by addition of the Rifampicin-Dabigatran Pgp-induction DDI study data. 

The dissolution of capsules was implemented via an empirical Weibull function using the Weibull parameters from the original model by [Moj et al. 2019](#main-references). 

### Distribution <a id="model-parameters-and-assumptions-distribution"></a>

...

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `PK-Sim Standard`. 

...

### Metabolism and Elimination <a id="model-parameters-and-assumptions-metabolism-and-elimination"></a>

...

### Automated Parameter Identification <a id="model-parameters-and-assumptions-parameter-identification"></a>

This is the result of the final parameter identification.

| Model Parameter      | Optimized Value | Unit |
| -------------------- | --------------- | ---- |
| `PK-Sim parameter 1` |                 |      |
| `PK-Sim parameter 2` |                 |      |
| `PK-Sim parameter 3` |                 |      |
| `PK-Sim parameter 4` |                 |      |

