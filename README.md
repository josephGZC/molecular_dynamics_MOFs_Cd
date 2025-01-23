![fig_cd_plots_coo_batch_2](https://github.com/user-attachments/assets/e62560ea-894b-42f3-99ae-5b6fa7da16fd)![fig_cd_plots_h_oh_cooh_batch_2](https://github.com/user-attachments/assets/f1fef1d0-1a80-4c7b-acd3-0af61d967cea)# **Investigating the Removal of Cadmium from Water through UiO-66 Derivatives using Molecular Dynamics**

Contents
- [Overview](#overview)
- [Python Scripts](#python-scripts)

## Overview
**Cadmium contamination** in water sources poses significant health and environmental risks, being linked to diseases like breast and lung cancer, bronchiolitis, and cerebral infection. Considering this, constant investigation on Cd(II) removal is essential.  Among water purification techniques, adsorption is most promising due to its cost-effectiveness, mild operating conditions, and high efficiency. Metal-organic frameworks (MOFs) have emerged as promising adsorbent, offering high porosity, ultrahigh surface area, and customizable functionalities, making them ideal for water purification.

**UiO-66**, a Zr-based MOF with exceptional aqueous stability, has demonstrated significant potential in water treatment. Composed of Zr<sub>6</sub>O<sub>4</sub>(OH)<sub>4</sub> metal clusters connected by 1,4-benzedicarboxylic acid (BDC) linkers, UiO-66 exhibits a robust structure ideal for heavy metal adsorption. Functional derivatives of UiO-66, such as UiO-66-NH<sub>2</sub>, have shown remarkable improvements in adsorption capacity, attributed to enhanced local electron density from functional groups like amino groups. Despite this progress, derivatives featuring hydroxyl and carboxylic groups remain underexplored for cadmium uptake. This study aims to address this gap by evaluating the cadmium adsorption performance of UiO-66-(OH) and UiO-66-(COOH) derivatives using molecular dynamics simulations. The research further seeks to analyze their adsorption mechanisms through distribution profiles, mobility analysis, radial distribution functions, and adsorption energy, providing insights into their viability for water purification applications.

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/5dcf5770-a601-4791-964e-0efe4f0d04ca">
</p>

Figure 1.1. The components (left) and unit cell (right) of UiO-66, where Zirconium, oxygen, carbon, and hydrogen atoms are represented by blue, red, dark gray, and light gray spheres, respectively. The metal cluster Zr6O4(OH)4 are represented by blue polyhedra. The tetrahedral and octahedral holes of UiO-66 are represented by pink and orange spheres, respectively.

## Python Scripts
The current repository contains some of the scripts used for this study. Specifically the python scripts that analyze percent removal, radial distribution function, and coordinate density.

[Open the Data File](plot-script_heatmap-coordinate/jup_rep_heatmap.ipynb)


<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/3be08deb-8fae-43bd-9d48-711d785f31c2">
</p>

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/eaeba421-311c-4059-9bff-c03796fe4c2e">
</p>



<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/100c6703-440a-447f-a2d3-0558fccb75b4" alt="Image 1" width="300">
  <img src="https://github.com/user-attachments/assets/4d497791-bf1e-4e5c-a425-7e78cd2ef319" alt="Image 2" width="300">
</div>

