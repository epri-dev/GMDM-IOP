# GMDM-IOP
Official Grid Model Data Management (GMDM) profile repository used by EPRI's Vendor Forum and related tooling.

This repository contains the RDFS profile artifacts, example instance data, and supporting files used for validating and demonstrating GMDM exchange profiles.

## Repository layout
- Information Model/  Enterprise Architect model file used as a reference: CIM_Grid18v15_Enterprise14v04_Market04v18_GMDM_v1.3.eap.
- Profiles/  RDFS profile artifacts (*.rdfs, *.schema.json) that define exchange profiles.
- Instance Data/  Example CIM instance XML files and exports used for testing and examples.
  - distribution/ and 	ransmission/ subfolders each include a 9500node_exports.ipynb notebook demonstrating how the test feeder exports were generated/inspected.

## Notebooks
Two Jupyter Notebooks are provided to inspect and work with the example instance data:
- Instance Data/distribution/9500node_exports.ipynb
- Instance Data/transmission/9500node_exports.ipynb

How to run the notebooks locally:
1. Install Python 3.8+ and Jupyter Lab/Notebook.
2. (Optional) Create and activate a virtual environment:
`powershell
python -m venv .venv
.\\.venv\\Scripts\\Activate.ps1
`
3. Install common packages (adjust as needed for the notebook code):
`powershell
pip install jupyterlab ipywidgets lxml
`
4. Start Jupyter:
`powershell
jupyter lab
`
5. Open one of the 9500node_exports.ipynb notebooks and run the cells.

Notes:
- The notebooks use standard Jupyter widgets and file dialogs; install ipywidgets to ensure UI elements work.
- The Information Model folder contains an Enterprise Architect .eap file for reference only and is not required to run the notebooks.

## License
See LICENSE at the repository root for license details.
