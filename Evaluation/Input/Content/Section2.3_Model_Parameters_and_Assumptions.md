### Absorption <a id="model-parameters-and-assumptions-absorption"></a>

All clinical studies included in this model were administered intravenously as a bolus or short infusion, directly into the venous blood compartment. No absorption process is included in the model structure.

### Distribution <a id="model-parameters-and-assumptions-distribution"></a>

Morphine, M6G, and M3G were parameterized with albumin as plasma protein binding partner, using the fraction unbound values described in [Section 2.2](#methods-data).

The organ-plasma partition coefficient and cellular permeability calculation methods for morphine and M6G (`Rodgers and Rowland` and `Charge dependent Schmitt`) were adopted from the model by Schaefer et al. ([Schaefer 2018](#main-references)). For M3G, the available methods built in PK-Sim were tested in a categorial parameter identification against the model-building data. The observed data were best described using `Rodgers and Rowland` for the partition coefficients and `PK-Sim Standard` for the cellular permeability.

### Metabolism and Elimination <a id="model-parameters-and-assumptions-metabolism-and-elimination"></a>

Morphine is eliminated by two parallel first-order UGT2B7 pathways, forming M6G and M3G, respectively, and by a minor first-order CYP3A4 pathway. M6G and M3G are eliminated renally by glomerular filtration and M6G additionally undergoes active first-order tubular secretion, while no active tubular secretion is assumed for M3G.

### Automated Parameter Identification <a id="model-parameters-and-assumptions-parameter-identification"></a>

The intrinsic clearances of morphine via CYP3A4, UGT2B7 (→ M6G), and UGT2B7 (→ M3G) were identified simultaneously against the model-building data ([Säwe 1985](#main-references), [Crews 2001](#main-references)). The specific organ permeabilities of morphine and M6G and the M6G tubular secretion were taken from the model by Schaefer et al. ([Schaefer 2018](#main-references)), where they were fitted to data from Lötsch et al. ([Lötsch 2002](#main-references)).

| Model Parameter                                  | Unit   | Source                                  |
| ------------------------------------------------ | ------ | --------------------------------------- |
| Morphine – CYP3A4 – Intrinsic clearance          | l/min  | Parameter identification (this work)    |
| Morphine – UGT2B7 (→ M6G) – Intrinsic clearance  | l/min  | Parameter identification (this work)    |
| Morphine – UGT2B7 (→ M3G) – Intrinsic clearance  | l/min  | Parameter identification (this work)    |
| Morphine – Pcell – Specific organ permeability   | cm/min | [Schaefer 2018](#main-references)       |
| M6G – Pcell – Specific organ permeability        | cm/min | [Schaefer 2018](#main-references)       |
| M6G – TS – Tubular secretion                     | l/min  | [Schaefer 2018](#main-references)       |
