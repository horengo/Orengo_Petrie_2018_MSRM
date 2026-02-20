# MSRM
### An algorithm to make visible subtle (not only) topographic changes at different scales

MSRM can be used to make visible near-invisible changes in Digital Surface Models or Digital Terrain Models. MSRM is different from other multi-scale microtopographic visualisation algortihms beccasue it produces a single-band raster, which makes it ideal for combination with other rasters (as a background for visualisation or as part or a multiband raster used in methods such as ML/ML-based classification). It can also be applied to different types of rasters, for example, when applied to each band of RGB images, it makes evident inperceptible changes in colour, imporving local contrast.

<img width="903" height="448" alt="Sent2" src="https://github.com/user-attachments/assets/5b428500-66c9-439c-9dfa-cc3bb66f09aa" />
<img width="903" height="448" alt="MSRM_RGB" src="https://github.com/user-attachments/assets/2d652c41-c764-4e7f-afdc-2fee5a7fb721" />


The Multi-Scale Relief Model script was originally published in Earth Surf. Process. Landf. (2018), 43(6): 1361-1369.
In this implementation it has been pdated with:
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
