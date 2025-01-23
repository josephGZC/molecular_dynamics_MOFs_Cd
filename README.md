# **Investigating the Removal of Cadmium from Water through UiO-66 Derivatives using Molecular Dynamics**

The following repository contains some of the jupyter lab python scripts I used in the simulation of UiO-66 and cadmium.

**Contents** 
- [Overview](#overview)
- [Python Scripts](#python-scripts)

## Overview
**Cadmium contamination** in water sources poses significant health and environmental risks, being linked to diseases like breast and lung cancer, bronchiolitis, and cerebral infection. Considering this, constant investigation on Cd(II) removal from water is essential.  Among water purification techniques, adsorption is most promising due to its cost-effectiveness, mild operating conditions, and high efficiency. Metal-organic frameworks (MOFs) have emerged as promising adsorbents, offering high porosity, ultrahigh surface area, and customizable functionalities.

**UiO-66**, a Zr-based MOF with exceptional aqueous stability, has demonstrated significant potential in water treatment. Composed of Zr<sub>6</sub>O<sub>4</sub>(OH)<sub>4</sub> metal clusters connected by 1,4-benzedicarboxylic acid (BDC) linkers, UiO-66 exhibits a robust structure ideal for heavy metal adsorption. Functional derivatives of UiO-66, such as UiO-66-NH<sub>2</sub>, have shown remarkable improvements in adsorption capacity, attributed to enhanced local electron density from functional groups like amino groups. Despite this progress, derivatives featuring hydroxyl and carboxylic groups remain underexplored for cadmium uptake. This study aims to address this gap by evaluating the cadmium adsorption performance of UiO-66-(OH) and UiO-66-(COOH) derivatives using molecular dynamics simulations. The research further seeks to analyze their adsorption mechanisms through distribution profiles, mobility analysis, radial distribution functions, and adsorption energy, providing insights into their viability for water purification applications.

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/5dcf5770-a601-4791-964e-0efe4f0d04ca">
</p>
Figure 1.1. The components (left) and unit cell (right) of UiO-66, where Zirconium, oxygen, carbon, and hydrogen atoms are represented by blue, red, dark gray, and light gray spheres, respectively. The metal cluster Zr6O4(OH)4 are represented by blue polyhedra. The tetrahedral and octahedral holes of UiO-66 are represented by pink and orange spheres, respectively.

## Simulation Set-up
UiO-66 and several of its derivatives where investigated. Specifically, UiO-66-(OH), UiO-66-(COOH), UiO-66-(COOH)<sub>2</sub>, UiO-66-(COOH)<sub>3</sub>, and UiO-66-(COOH)<sub>4</sub>. MOFs were positioned at the center of the simulation box as shown in Figure 1. A non-MOF region extends 20 Å from the negative and positive z-axes of the MOFs, which is referred to as the empty region.  For each MOF, four systems were packed with different Cd(II) number densities and equal number of water molecules.  Water molecules were randomly inserted throughout the entire system, while Cd(II) insertion was restricted to the empty region.

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/1c1a2328-6dc4-4de1-bdf7-96653db6515c">
</p>
Figure 2. System snapshot showing UiO-66 packed with water (light blue sphere connected to white spheres) and Cd(II) (yellow spheres). In the MOF region, zirconium, oxygen, carbon, and hydrogen atoms are represented by blue, red, dark gray, and light gray spheres, respectively.The metal cluster nodes Zr6O4(OH)4 are represented by blue polyhedra.

## Simulation Analysis
In analyzing the adsorption performance of the investigated MOFs, the amount of Cd adsorbed and the mechanism of adsorption is explored. The performance was evaluated by counting the number of Cd atoms found inside the MOFs, while adsorption behavior was explored by looking into coordinate position and MOF atom preference (other analysis such as adsorption energy and mean square displacement were not included here). Several python scripts were created to analyze the trajectory output from the simulations. Pandas was used to process CSV files whie seaborn was employed to generate plots. 

* [Percent Removal](plot-script_percent-removal/jup_rep_dyn_plots.ipynb)
* [Density Map](plot-script_heatmap-coordinate/jup_rep_heatmap.ipynb)
* [Radial Distribution Function](plot-script_radial-distribution-function/jup_rep_rdf_plots.ipynb) 

### Percent Removal

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/3be08deb-8fae-43bd-9d48-711d785f31c2">
</p>

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/eaeba421-311c-4059-9bff-c03796fe4c2e">
</p>

### Density Map
<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/100c6703-440a-447f-a2d3-0558fccb75b4" alt="Image 1" width="300">
  <img src="https://github.com/user-attachments/assets/4d497791-bf1e-4e5c-a425-7e78cd2ef319" alt="Image 2" width="300">
</div>

### Radial Distribution Function
<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/f5347795-22cd-4001-812c-af8d54f2a0b4">
</p>
<p align="center" width="100%">
    <img width="59.6%" src="https://github.com/user-attachments/assets/670ffb80-35cc-47b8-925a-9a1308a45f70">
</p>
