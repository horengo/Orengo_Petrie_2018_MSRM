# MSRM


Multi-Scale Relief Model script originally published in Earth Surf. Process. Landf. (2018), 43(6): 1361-1369
Updated with:
 - Parallel excution for each generated surface
 - Admits both projected and geographic (degrees) CRS
 - Visualisation of the resulting MSRM

## Setting up the environment

Create and activate an env using the provided YAML file: <br>
```
conda env create -f environment_MSRM.yml  # Creates the environemt and installs the pinned packages
conda activate MSRM  # Activates the environment
python -m ipykernel install --user --name MSRM --display-name "MSRM"  # Optional: registers your current Python environment as a selectable Jupyter kernel. No need to use if you are going to lauch Jupyter from MSRM environment (the YAML file installs Jupyter Lab/Notebook) <br>
```
