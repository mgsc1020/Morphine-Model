### Absorption <a id="model-parameters-and-assumptions-absorption"></a>

All clinical studies included in this model were administered intravenously as a bolus or short infusion, directly into the venous blood compartment. No absorption process is included in the model structure.

### Distribution <a id="model-parameters-and-assumptions-distribution"></a>

Morphine, M6G, and M3G were parameterized with albumin as plasma protein binding partner, using the fraction unbound values described in [Section 2.2](#methods-data).

The organ-plasma partition coefficient and cellular permeability calculation methods for morphine and M6G (`Rodgers and Rowland` and `Charge dependent Schmitt`) were adopted from the model by Schaefer et al. ([Schaefer 2018](#main-references)). For M3G, the available methods built in PK-Sim were tested in a parameter identification against the plasma concentration-time profiles of morphine, M6G, and M3G from [Säwe 1985](#main-references) and [Crews 2001](#main-references). The observed data were best described using `Rodgers and Rowland` for the partition coefficients and `PK-Sim Standard` for the cellular permeability.

### Metabolism and Elimination <a id="model-parameters-and-assumptions-metabolism-and-elimination"></a>

Morphine is eliminated by two parallel first-order UGT2B7 pathways, forming M6G and M3G, respectively, and by a minor first-order CYP3A4 pathway. M6G and M3G are eliminated renally by glomerular filtration and M6G additionally undergoes active first-order tubular secretion, while no active tubular secretion is assumed for M3G.

Approximately 90% of a morphine dose is metabolized, while 10% is excreted unchanged in urine and 7–10% is recovered as glucuronides in feces. Of the dose, 45–55% is converted to M3G, 10–15% to M6G, and approximately 5% to normorphine via CYP3A4 ([ScienceDirect Topics](#main-references)). These values were corrected for incomplete recovery, resulting in 11% of the dose excreted as unchanged morphine, 58% as M3G, 16% as M6G, and 5% as normorphine (89% in total). Accordingly, the fractions of the dose metabolized (fm) were set to 0.58 for UGT2B7 (→ M3G), 0.16 for UGT2B7 (→ M6G), and 0.05 for CYP3A4. The fm of 0.58 for M3G is based on the recovered M3G and represents a lower limit: M3G undergoes enterohepatic circulation ([Hasselström 1993](#main-references)), during which part of the M3G formed is converted back to morphine and eliminated unchanged in feces, eliminated as glucuronide in feces, or metabolized again in the liver. The actual fraction of morphine converted to M3G is therefore likely higher, at approximately 70% (90% total metabolism − 15% M6G − 5% normorphine). Modeling the enterohepatic circulation of M3G was beyond the scope of this work; the fm of 0.58 was therefore used as a conservative estimate.

The CYP3A4 pathway accounts for only a minor fraction of morphine elimination. To avoid identifiability issues, its intrinsic clearance was fixed at 0.25 l/min, resulting in approximately 5% of the dose being metabolized to normorphine.

### Automated Parameter Identification <a id="model-parameters-and-assumptions-parameter-identification"></a>

The intrinsic clearances of morphine via UGT2B7 (→ M6G) and UGT2B7 (→ M3G) were identified simultaneously against the morphine plasma concentration-time profiles of the model-building data ([Section 2.2.2](#clinical-data)). Because plasma concentrations alone do not inform how morphine clearance is split between the metabolic pathways, the simulated fm via each pathway was fitted simultaneously against the fm values described above.

The specific organ permeabilities of morphine and M6G and the M6G tubular secretion were taken from the model by Schaefer et al. ([Schaefer 2018](#main-references)), where they were fitted to data from Lötsch et al. ([Lötsch 2002](#main-references)).

| Model Parameter                                  | Unit   | Source                                  |
| ------------------------------------------------ | ------ | --------------------------------------- |
| Morphine – CYP3A4 – Intrinsic clearance          | l/min  | Fixed (fm ≈ 0.05)                       |
| Morphine – UGT2B7 (→ M6G) – Intrinsic clearance  | l/min  | Parameter identification (this work)    |
| Morphine – UGT2B7 (→ M3G) – Intrinsic clearance  | l/min  | Parameter identification (this work)    |
| Morphine – Pcell – Specific organ permeability   | cm/min | [Schaefer 2018](#main-references)       |
| M6G – Pcell – Specific organ permeability        | cm/min | [Schaefer 2018](#main-references)       |
| M6G – TS – Tubular secretion                     | l/min  | [Schaefer 2018](#main-references)       |
