### Absorption <a id="model-parameters-and-assumptions-absorption"></a>

All clinical studies included in this model were administered intravenously as a bolus or short infusion, directly into the venous blood compartment. No absorption process is included in the model structure.

### Distribution <a id="model-parameters-and-assumptions-distribution"></a>

Morphine, M6G, and M3G were parameterized with albumin as plasma protein binding partner, using the fraction unbound values described in [Section 2.2](#methods-data).

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim (including `Rodgers and Rowland`, `Berezhkovskiy`, `Poulin and Theil`, and `Schmitt`), observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` for all three compounds, and the cellular permeability calculation by `Charge dependent Schmitt` for morphine and M6G, and `PK-Sim Standard` for M3G.

### Metabolism and Elimination <a id="model-parameters-and-assumptions-metabolism-and-elimination"></a>

Morphine is eliminated by two parallel first-order UGT2B7 pathways, forming M6G and M3G, respectively, and by a minor first-order CYP3A4 pathway. M6G and M3G are eliminated renally by glomerular filtration and M6G additionally undergoes active first-order tubular secretion, while no active tubular secretion is assumed for M3G.

### Automated Parameter Identification <a id="model-parameters-and-assumptions-parameter-identification"></a>

This is the result of the final parameter identification.

| Model Parameter         | Unit  |
| ---------------------------------------------- | ----- |
| Morphine – Pcell – Specific organ permeability            | cm/min |
| Morphine – CYP3A4 – Intrinsic clearance                    | l/min |
| Morphine – UGT2B7 (→ M6G) – Intrinsic clearance            | l/min |
| Morphine – UGT2B7 (→ M3G) – Intrinsic clearance             | l/min |
| M6G – Pcell – Specific organ permeability                    | cm/min |
| M6G – TS – Tubular secretion                    | l/min |
