# DINEOF analysis of 2021 MODIS aerosol optical depth

This repository contains a Jupyter notebook for analyzing weekly 2021 MODIS aerosol optical depth (AOD) data and evaluating gap-filled fields produced with DINEOF (Data Interpolating Empirical Orthogonal Functions). The notebook covers data preparation, reconstruction checks, missing-data summaries, maps, spatial diagnostics, validation experiments, and EOF analysis.

## Notebook

- [`Dineof_2021.ipynb`](Dineof_2021.ipynb) — the analysis notebook. It was developed in Google Colab and reads and writes files in Google Drive.

## Data and setup

The input `.npz` datasets and generated figures/results are **not included** in this repository. The notebook refers to Google Drive paths under `/content/drive/MyDrive/`, including `MODIS_2021_Weekly_Averages.npz` and `DINEOF_2021_REVISED_BBOX_LANDMASK/MODIS_2021_DINEOF_Revised_Final.npz`. To run it, provide these datasets and update the paths for your Drive layout.

Open the notebook in Google Colab, mount Google Drive when prompted, install any missing Python packages, and run cells in order. The code uses NumPy, pandas, Matplotlib, SciPy, scikit-learn, and TensorLy. Some later cells depend on files and variables created by earlier cells, so the notebook is not currently a standalone run from a fresh environment without its external data and outputs.

## Study area

The notebook documents a study region of approximately 18–35°N and 73–90°E, with 52 weekly layers and 2 × 2 spatial aggregation. Its quality-control cells compare original observations with reconstructed values and examine missingness and spatial artifacts.
