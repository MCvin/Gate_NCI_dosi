# Gate_NCI_dosi

```
GATE macro for nuclear medicine dosimetry with the NCI voxel models  

Author: Maxime Chauvin, maxime.chauvin@inserm.fr
Last revision: 22-09-2020

Usage example, for mono energetic source:
  Gate -a [model,00F][source_id,95][particle,gamma][energy,1][nb,1e5][job,1] mac/main.mac

Inputs:
  - data/activity_ranges/ActivityRange_{source_id}.dat
  - data/NCI_{model}_GateMaterials.db
  - data/NCI_{model}_LabelsToMaterials.txt
  - data/NCI_models/NCI_{model}_*.mhd
  - data/NCI_models/NCI_{model}_*.raw

Outputs:
  - output/{job}_{model}-DoseByRegions.txt
  - output/{job}_{model}-Dose.mhd
  - output/{job}_{model}-Dose.raw
  - output/{job}_{model}-Dose-Squared.mhd
  - output/{job}_{model}-Dose-Squared.raw
  - output/{job}_{model}-Dose-Uncertainty.mhd
  - output/{job}_{model}-Dose-Uncertainty.raw
  - output/{job}_{model}-stats.txt
```
