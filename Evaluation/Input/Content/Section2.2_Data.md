### In vitro / physico-chemical Data <a id="invitro-and-physico-chemical-data"></a>

A literature search was performed to collect available information on the physicochemical properties of morphine, morphine-6-glucuronide (M6G), and morphine-3-glucuronide (M3G). The information used in the model is summarized in the tables below.

**Morphine**

| **Parameter**   | **Unit** | **Value** | Source                                     | **Description**                                 |
| :-------------- | -------- | --------- | ------------------------------------------ | ----------------------------------------------- |
| MW              | g/mol    | 285.34    | [DrugBank](#main-references)               | Molecular weight                                |
| pK<sub>a</sub> (base) |    | 8.21      | [DrugBank](#main-references)               | Acid dissociation constant                      |
| logP            | Log Units | 0.9 / 0.89 | [Avdeef 1996](#main-references)           | Partition coefficient between octanol and water |
| Solubility (pH 7) | mg/l   | 149.0     | [Yalkowsky 1992](#main-references)         | Aqueous solubility                              |
| fu              | %        | 65        | [Olsen 1975](#main-references)             | Fraction unbound in plasma                      |

**Morphine-6-glucuronide (M6G)**

| **Parameter**   | **Unit** | **Value** | Source                                     | **Description**                                 |
| :-------------- | -------- | --------- | ------------------------------------------ | ----------------------------------------------- |
| MW              | g/mol    | 461.5     | [DrugBank](#main-references)               | Molecular weight                                |
| pK<sub>a</sub> (base) |    | 8.22      | [Eissing 2012](#main-references)           | Acid dissociation constant                      |
| logP            | Log Units | 0.79     | [Eissing 2012](#main-references)           | Partition coefficient between octanol and water |
| Solubility (pH 7) | mg/l   | 1.0       | [DrugBank](#main-references)               | Aqueous solubility                              |
| fu              | %        | 83        | [Eissing 2012](#main-references)           | Fraction unbound in plasma                      |

**Morphine-3-glucuronide (M3G)**

| **Parameter**   | **Unit** | **Value** | Source                                     | **Description**                                 |
| :-------------- | -------- | --------- | ------------------------------------------ | ----------------------------------------------- |
| MW              | g/mol    | 461.46    | [PubChem](#main-references)                | Molecular weight                                |
| pK<sub>a</sub> (acid) |    | 2.83      | [Andersen 2003](#main-references)          | Acid dissociation constant                      |
| logP            | Log Units | -0.63    | [HMDB 2007](#main-references)                         | Partition coefficient between octanol and water (predicted, ALOGPS) |
| Solubility (pH 7) | g/l    | 9.06      | [HMDB 2007](#main-references)                         | Aqueous solubility (predicted, ALOGPS)          |
| fu              | %        | 85        | [Andersen 2003](#main-references)          | Fraction unbound in plasma                      |

### Clinical Data  <a id="clinical-data"></a>

A literature search was performed to collect available clinical data on morphine, M6G, and M3G plasma concentrations in healthy adults after intravenous administration of morphine or M6G. Five M3G plasma concentration datasets were identified in the literature; two were used for model building ([Säwe 1985](#main-references), [Crews 2001](#main-references)) and three for model verification ([Osborne 1990](#main-references), [Ferslew 2015](#main-references), [Stuart-Harris 2000](#main-references)). Although the Säwe et al. study was conducted in cancer patients rather than healthy volunteers, it was retained for model building because morphine and M3G pharmacokinetics observed in this population were in overall agreement with those observed in healthy volunteers.

#### Model Building <a id="model-building"></a>

The following studies were used for model building (training data):

| Publication                 | Arm / Treatment / Information used for model building |
| :-------------------------- | :---------------------------------------------------- |
| [Säwe 1985](#main-references) | Cancer patients, 2-minute intravenous infusion of 3.55 mg morphine; morphine and M3G plasma concentrations |
| [Crews 2001](#main-references) | Healthy volunteers, 5-minute intravenous infusion of 7.52 mg morphine; morphine, M6G, and M3G plasma concentrations |


#### Model Verification <a id="model-verification"></a>

The following studies were used for model verification:

| Publication                 | Arm / Treatment / Information used for model verification |
| :-------------------------- | :---------------------------------------------------- |
| [Lötsch 2002](#main-references) | Healthy volunteers, intravenous bolus of 5.64 mg morphine and intravenous bolus of 1 mg M6G; morphine and M6G plasma concentrations |
| [Westerling 1995](#main-references) | Healthy volunteers, 20-minute intravenous infusion of 7.59 mg morphine; morphine and M6G plasma concentrations |
| [Hoskin 1989](#main-references) | Healthy volunteers, 2-minute intravenous infusion of 3.76 mg morphine; individual morphine plasma concentrations |
| [Lötsch 1998](#main-references) | Healthy volunteers, weight-normalized intravenous bolus-plus-4h-infusion regimens of M6G (0.015+0.0288 to 0.044+0.088 mg/kg) and morphine (0.124+0.177 mg/kg), and a combined regimen; morphine and M6G plasma concentrations |
| [Dershwitz 2000](#main-references) | Healthy volunteers, 7-minute intravenous infusion of 6.62 mg morphine; morphine plasma concentrations |
| [Stuart-Harris 2000](#main-references) | Healthy volunteers, 4.8-minute intravenous infusion of 7.52 mg morphine; morphine, M6G, and M3G plasma concentrations\* |
| [Baillie 1989](#main-references) | Healthy volunteers, 10-minute intravenous infusion of 7.52 mg morphine; morphine plasma concentrations |
| [Osborne 1990](#main-references) | Healthy volunteers, intravenous bolus of 3.76 mg morphine; morphine, M6G, and M3G plasma concentrations |
| [Ferslew 2015](#main-references) | Healthy subjects, 5-minute intravenous infusion of 3.76 mg morphine; morphine and M3G plasma concentrations |

\*PK profiles were corrected to a dose of 10 mg/70 kg ([Stuart-Harris 2000](#main-references)).

Morphine sulphate and morphine hydrochloride doses were converted to morphine base.