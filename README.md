# Morphine-Model
Whole-body PBPK model of morphine and its glucuronide metabolites morphine-6-glucuronide (M6G) and morphine-3-glucuronide (M3G).

## Repository files
This repository contains:

- a PK-Sim snapshot (*.json) file of the current whole-body PBPK model of morphine, M6G, and M3G
- static content (e.g. text blocks, *.md files) as inputs for an evaluation plan
- an evaluation plan (Evaluation/Input/evaluation_plan.json) to create an evaluation report using the snapshot and static text blocks to display the performance of the model

The model was developed and evaluated for morphine, M6G, and M3G using plasma concentration data from several clinical studies in adults. The model is based on a modified version of the morphine and M6G PBPK model published by Schaefer et al. [1], extended to include M3G and additional clinical datasets.
For morphine, the model was developed and evaluated against intravenous bolus and infusion administration (dosing range of 3.55 mg to 7.59 mg, and a weight-normalized bolus-plus-4h-infusion regimen of 0.124+0.177 mg/kg).
For M6G, the model was evaluated against direct intravenous administration (1 mg bolus and weight-normalized bolus-plus-4h-infusion regimens of 0.015+0.0288 to 0.044+0.088 mg/kg) and as the metabolite formed from the administered morphine doses.
For M3G, the model was developed and evaluated as the metabolite formed from intravenous morphine doses of 3.55 mg to 7.52 mg. 
The model was developed and evaluated for intravenous administration only. No clinical data after direct administration of M3G were used.

The PK-Sim snapshot file contains simulations and the observed data of all clinical studies used for model development and evaluation.

## Code of conduct
Everyone interacting in the Open Systems Pharmacology community (codebases, issue trackers, chat rooms, mailing lists etc...) is expected to follow the Open Systems Pharmacology [code of conduct](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODE_OF_CONDUCT.md#contributor-covenant-code-of-conduct).

## Contribution
We encourage contribution to the Open Systems Pharmacology community. Before getting started please read the [contribution guidelines](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CONTRIBUTING.md#ways-to-contribute). If you are contributing code, please be familiar with the [coding standard](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODING_STANDARDS.md#visual-studio-settings).

## License
The model code is distributed under the [GPLv2 License](https://github.com/Open-Systems-Pharmacology/Suite/blob/develop/LICENSE).

## References
[1] Schaefer N, Moj D, Lehr T, Schmidt PH, Ramsthaler F. The feasibility of physiologically based pharmacokinetic modeling in forensic medicine illustrated by the example of morphine. Int J Legal Med. 2018 Mar;132(2):415-424. doi: 10.1007/s00414-017-1754-8.
