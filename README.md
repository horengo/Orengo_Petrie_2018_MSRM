# MSRM
### An algorithm to make visible subtle (not only) topographic changes at different scales

MSRM can be used to make visible near-invisible changes in Digital Surface Models or Digital Terrain Models. MSRM is different from other multi-scale microtopographic visualisation algortihms beccasue it produces a single-band raster, which makes it ideal for combination with other rasters (as a background for visualisation or as part or a multiband raster used in methods such as ML/ML-based classification). It can also be applied to different types of rasters, for example, when applied to each band of RGB images, it makes evident inperceptible changes in colour, imporving local contrast.

<img width="500" height="200" alt="Sent2" src="https://github.com/user-attachments/assets/cc074f8b-7854-443e-b2a4-e37e89fd2e5a" />
<img width="500" height="200" alt="MSRM_RGB" src="https://github.com/user-attachments/assets/38867c97-3fad-497d-95cb-bef020f32be5" />

*Comparison between multitemporal cloud-free Harmonised Sentinel 2 image (2&sigma; stretched) - top - and MSRM of the same image (2&sigma; stretched) - down*

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
