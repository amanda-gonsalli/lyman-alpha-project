# Lyman-alpha Research Project

This repository contains exploratory notebooks developed during an ongoing, year-long research project through the University of Michigan's Undergraduate Research Opportunity Program (UROP), under the guidance of postdoctoral researcher Ming-Feng Ho. The notebooks document progress in spectral analysis, comparisons across redshifts, and visualization of cosmological simulation data. The notebook guide will grow as new analyses are added.

## Official project description

### Guiding question: Do high-column density absorbers contain useful information for Lyman-alpha forest inference?

The Lyman-alpha forest is widely used to constrain cosmology and the thermal state of the intergalactic medium at redshifts z ~ 2-5. In standard analyses, the target signal is usually taken to be the low-density IGM, while high-column density absorbers (HCDs), including Lyman limit systems (LLSs) and damped Lyman-alpha absorbers (DLAs), are treated as contaminants and masked out.

This treatment is practical, but it is also an idealization. In real quasar spectra, absorption from the low-density IGM, circumgalactic gas, HCD systems, and metals all appear along the same line of sight. Separating these components is difficult in practice and depends on imperfect catalogs or masking procedures. For example, DLA masking requires highly complete and highly pure DLA finders, but even the best current catalogs are far from perfect, especially at modest signal-to-noise.

A more basic question is whether masking HCD systems is throwing away useful information. HCD absorbers are not random nuisances. Their abundance and redshift evolution depend on astrophysical processes such as the UV background and galaxy feedback, and they may also carry information relevant for cosmological inference. The usual approach is therefore convenient, but not obviously optimal.

This project asks a simple question: if we include HCD systems rather than remove them, do we gain or lose information in Lyman-alpha forest inference? The student will reproduce and extend recent simulation-based inference (SBI) analyses of the 1D Lyman-alpha forest power spectrum using hydrodynamical simulation suites, including CAMELS (IllustrisTNG and SIMBA) and, if feasible, PRIYA. Two inference setups will be compared: one using Lyman-alpha forest statistics constructed after removing HCD contributions, and one using statistics that include both the forest and HCD population.

The main goal is to quantify how parameter inference changes between these two cases. In particular, the project will test whether including HCDs improves constraints, introduces additional degeneracies, or mainly reduces bias relative to analyses that ignore them. The broader aim is to clarify whether HCD absorbers should be treated purely as contamination, or as part of the signal space of Lyman-alpha forest cosmology.

## Notebook guide

| Notebook | Purpose |
| --- | --- |
| [Reading_spectra.ipynb](Reading_spectra.ipynb) | Explore the structure of CAMELS spectra files and plot transmitted flux, optical depth, and neutral hydrogen column density along simulated sightlines. |
| [Comparing_snapshots.ipynb](Comparing_snapshots.ipynb) | Compare spectra and column densities across simulation snapshots to explore changes with redshift. |
| [Visualization_matter_distribution.ipynb](Visualization_matter_distribution.ipynb) | Explore CAMELS 3D grid data through perpendicular slices and 3D visualizations, with optional interactive views. |

## Data

The notebooks use data from [CAMELS (Cosmology and Astrophysics with MachinE Learning Simulations)](https://camels.readthedocs.io/en/latest/). The local `Datasets/` folder is excluded from Git and is **not included in this repository**. Download the required files separately and place them in the layout below. Generated figures and exports are saved locally in `outputs/`, which is also excluded from Git.

