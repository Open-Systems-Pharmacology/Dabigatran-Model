The general concept of building a PBPK model has previously been described by Kuepfer et al. ([Kuepfer 2016](#main-references)). Regarding the relevant anthropometric (height, weight) and physiological parameters (e.g. blood flows, organ volumes, binding protein concentrations, hematocrit, cardiac output) in adults was gathered from the literature and has been previously published ([PK-Sim Ontogeny Database Version 7.3](#main-references)). The information was incorporated into PK-Sim® and was used as default values for the simulations in adults.

The  applied activity and variability of plasma proteins and active processes that are integrated into PK-Sim® are described in the publicly available PK-Sim® Ontogeny Database Version 7.3 ([Schlender 2016](#main-references)) or otherwise referenced for the specific process.

The PBPK model was developed using a stepwise modeling strategy. First, an intravenous dabigatran model was established to describe distribution and elimination processes, including UGT2B15-mediated glucuronidation of dabigatran to dabigatran glucuronide as well as the renal clearance of both.

Second, the model was extended to include the orally administered prodrug dabigatran etexilate. This step required incorporation of Pgp-mediated transport affecting its absorption and CES1/CES2-mediated prodrug activation to produce dabigatran. 

The respective contributions of CES1 and CES2 were informed by data from the RE-LY trial ([Paré 2013](#main-references)), reporting that patients carrying 2 minor CES1 alleles (modeled as complete loss of CES1 activity) show a 28% reduction of their total dabigatran plasma concentration trough values (total dabigatran = dabigatran + dabigatran glucuronide). 

While the original model considered data of 2 different clinical DDI studies (rifampicin-mediated Pgp induction ([Härtter 2012](#main-references)) and clarithromycin-mediated Pgp inhibition ([Delavenne 2013](#main-references)), for the model update data of 7 further clinical DDI trials were used, adding Pgp inhibition by rifampicin (n=2), itraconazole (n=1), verapamil (n=1), and additional clarithromycin studies (n=3) (please see the DDI qualification report ([https://github.com/Open-Systems-Pharmacology/COMPOUND-Model](https://github.com/Open-Systems-Pharmacology/COMPOUND-Model)). 

Unknown parameters were identified using the PK‑Sim® Parameter Identification module. Model evaluation included comparison of predicted versus observed concentration–time profiles, goodness-of-fit plots, and geometric mean fold error (GMFE) analysis.

Details about input data (physicochemical, *in vitro* and clinical) can be found in  [Section 2.2](#methods-data).

Details about the structural model and its parameters can be found in  [Section 2.3](#model-parameters-and-assumptions).

