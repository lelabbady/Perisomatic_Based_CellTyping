# Perisomatic_Based_CellTyping
Repository to accompany the manuscript Perisomatic Ultrastructure Efficiently Classifies Cells in Mouse Cortex (Elabbady 2024). The tutorials in this repository are aimed to recapitulate the figures and analyses from the manuscript. 

For feature extraction pipelines, please look at the following repositories:
- Nucleus and Soma Extraction
- Spine Extraction from mesh objects
- Post-Synaptic Shape Feature Extraction

## Installation

To run the tutorials provided in this repository please follow the installation instructions found at MicronsBinder. The conda environment file has been provided here as well.

## Datasets

This repository comes with several public data files. Filenames and definitions are provided below:
  - microns_SomaData_AllCells_v661.pkl This file contains the nucleus and soma features for all 94,010 cells presented in the manuscript. Note that this includes all predicted neurons and non-neurons but excludes any objects predicted as errors. Details about how each feature was calculated can be found in the Methods section under 'Generatuing Nucleus and Soma Features'
  - inhibitory_perisomatic_feats_v661.pkl This file contains the nucleus, soma, and PSS features that were extracted for all 6,805 predicted inhibitory neurons. Note that the numbers in each shape column denotes the number of objects of that shape detected within a given spatial bin. So for example, a value of 5 in shape_2_0_15000 means that a given cell had 5 instances of Shape 2 between 0-15 microns from the soma center point.
