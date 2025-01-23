# **Investigating the Removal of Cadmium from Water through UiO-66 Derivatives using Molecular Dynamics**

The following repository contains some of the jupyter lab python scripts I used in the simulation of UiO-66 and cadmium.

### Contents

🔖 Sections
- [Overview](#overview)
- [Simulation Setup](#simulation-setup)
- [Simulation Analysis](#simulation-analysis)

🐍 Python Scripts
* [Percent Removal](plot-script_percent-removal/jup_rep_dyn_plots.ipynb)
* [Density Map](plot-script_heatmap-coordinate/jup_rep_heatmap.ipynb)
* [Radial Distribution Function](plot-script_radial-distribution-function/jup_rep_rdf_plots.ipynb)

## Overview
[[back to contents](#contents)]

Cadmium contamination in water sources poses significant health and environmental risks, being linked to diseases like breast and lung cancer, bronchiolitis, and cerebral infection. Considering this, constant investigation on Cd(II) removal from water is essential. Among water purification techniques, adsorption is most promising due to its cost-effectiveness, mild operating conditions, and high efficiency. 

Metal-organic frameworks (MOFs) have emerged as promising adsorbents, offering high porosity, ultrahigh surface area, and customizable functionalities. [UiO-66](https://doi.org/10.1021/ja8057953), a Zr-based MOF with exceptional aqueous stability, has demonstrated significant potential in water treatment. Composed of Zr<sub>6</sub>O<sub>4</sub>(OH)<sub>4</sub> metal clusters connected by 1,4-benzedicarboxylic acid (BDC) linkers, UiO-66 exhibits a robust structure ideal for heavy metal adsorption. 

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/5dcf5770-a601-4791-964e-0efe4f0d04ca">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 1</strong>. The components (left) and unit cell (right) of UiO-66, where zirconium, oxygen, carbon, and <br/>
    hydrogen atoms are represented by blue, red, dark gray, and light gray spheres, respectively. The <br/>  
    metal cluster Zr<sub>6</sub>O<sub>4</sub>(OH)<sub>4</sub> are represented by blue polyhedra. The tetrahedral
    and octahedral <br/> holes of UiO-66 are represented by pink and orange spheres, respectively.
</p>

This study aims to evaluate cadmium adsorption performance of UiO-66 and its hydroxyl and carboxylic derivatives (UiO-66-(OH) and UiO-66-(COOH)) using molecular dynamics simulations, wherein the functional group attachment affects the local electron density of the MOFs and subsequent attraction with Cd. The research further seeks to analyze their adsorption mechanisms through distribution profiles, mobility analysis, radial distribution functions, and adsorption energy, providing insights into their viability for water purification applications.

> 🔗 Polymers are simply the combination of single chemical units. </br>
> * Carbohydrates are polymers of sugars. </br>
> * DNA are polymers of nucleotides. </br>
> * MOFs are polymers of metals and organic compounds. </br>
> * UiO-66 (a MOF) is a polymer of Zr clusters and BDC linkers

## Simulation Setup
[[back to contents](#contents)]

UiO-66 and several of its derivatives where investigated. Specifically, UiO-66-(OH), UiO-66-(COOH), UiO-66-(COOH)<sub>2</sub>, UiO-66-(COOH)<sub>3</sub>, and UiO-66-(COOH)<sub>4</sub>. MOFs were positioned at the center of the simulation box as shown in Figure 1. A non-MOF region extends 20 Å from the negative and positive z-axes of the MOFs, which is referred to as the empty region.  For each MOF, four systems were packed with different Cd(II) number densities and equal number of water molecules.  Water molecules were randomly inserted throughout the entire system, while Cd(II) insertion was restricted to the empty region.

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/1c1a2328-6dc4-4de1-bdf7-96653db6515c">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 2</strong>. System snapshot showing UiO-66 packed with water (light blue sphere connected to <br/>
    white spheres) and Cd(II) (yellow spheres). In the MOF region, zirconium, oxygen, carbon, and <br/> 
    hydrogen atoms are represented by blue, red, dark gray, and light gray spheres, respectively. <br/> 
    The metal cluster nodes Zr<sub>6</sub>O<sub>4</sub>(OH)<sub>4</sub> are represented by blue polyhedra.
</p>

> 🛠️ The setup was prepared to answer the question, will Cd remain in water or will it go inside the MOFs?

## Simulation Analysis
[[back to contents](#contents)]

In analyzing the adsorption of the investigated MOFs, the <ins>performance of adosprtion</ins> and the <ins>mechanism of adsorption</ins> is explored. The performance was evaluated by counting the number of Cd atoms and water molecules found inside the MOFs, and subsequent calculation of  percent removal (i.e. percent of substance removed from the solution). A better-performing MOF correspond to adsorbing more Cd atoms (higher Cd percent removal) and adsoring less water molecules (lower water percent removal). Adsorption behavior was explored by looking into guest molecule (Cd or water) distribution and MOF atom preference (other analysis such as adsorption energy and mean square displacement were not included here). Several python scripts were created to analyze the trajectory output from the simulations. Pandas was used to process CSV files while seaborn was employed to generate plots. 

> 💻 **Analysis Flow Guide**
> * A. Determine adsorption performance from [Percent Removal](plot-script_percent-removal/jup_rep_dyn_plots.ipynb)
> * B. Determine guest molecule (Cd or Water) distribution [Density Map](plot-script_heatmap-coordinate/jup_rep_heatmap.ipynb)
> * C. Determine MOF atom interaction preference from [Radial Distribution Function](plot-script_radial-distribution-function/jup_rep_rdf_plots.ipynb) 

### A. Adsorption Performance

From all the simulations, the number of Cd(II) atoms within the MOF region and the empty region were plotted as a function of time as shown in Fig. 3 and 4. This was presented for all MOFs across varying initial Cd(II) concentration. The results show that after an abrupt entry of Cd(II) into the MOF region within the 1-ns mark, further adsorption showed only minor fluctuations. In all cases, Cd(II) concentration remained consistently higher in the MOF region compared to the empty region until the simulation endpoint. These observations demonstrate that Cd(II) has an affinity for adsorption onto the MOFs, suggesting that their passage into the MOF is driven by more than just the initial concentration gradient.

> 🟨 Where the Cd atoms adsrobed to the MOFs? ➡️ Yes, Cd atoms entered the MOFs and remained there until the end of the simulation.

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/3be08deb-8fae-43bd-9d48-711d785f31c2">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 3</strong>. Number of Cd(II) atoms adsorbed by UiO-66, UiO-66-OH, and UiO-66-COOH at different <br/> 
    initial Cd(II) content. Specifically, the total initial count are (a-c) 100 and (d-f) 150 atoms.
</p>

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/eaeba421-311c-4059-9bff-c03796fe4c2e">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 4</strong>. Number of Cd(II) atoms adsorbed by UiO-66-(COOH)<sub>2</sub>, UiO-66-(COOH)<sub>3</sub>, and <br/> 
    UiO-66-(COOH)<sub>4</sub> at different initial Cd(II) content. Specifically, the total initial count <br/> are (a-c) 100 and (d-f) 150 atoms.
</p>

When calculating percent removal in the system with initial Cd(II) atoms equal to 100, more than one MOF tied with the highest percent removal (Fig. 5). In that series, UiO-66-(COOH)<sub>2</sub> and UiO-66-(COOH)<sub>4</sub> achieved slightly higher percent removal values compared to the other MOFs. UiO-66-(COOH)<sub>4</sub> achieved slightly higher percent removal in 25 and 150 initial Cd(II) content. The highest percent removal obtained for UiO-66-(COOH)<sub>4</sub> was 88%.

Besides percent removal of Cd(II), percent removal of water was also explored as shown in Fig. 6. In this case, lower water adsorption is the desired outcome. Interestingly, while a distinct trend was not evident for Cd(II) percent removal across the incremental increase of carboxylic acid groups, a notable decrease in water adsorption was observed from UiO-66-(COOH) to UiO-66-(COOH)<sub>4</sub>. Given the significant difference in water percent removal across the investigated MOFs, UiO-66-(COOH)<sub>4</sub> is particularly effective at adsorbing Cd(II) while minimizing water uptake.

> 🟨 Are the MOFs siutable for Cd adsoprtion? ➡️ Yes, becase Cd adsorption of all MOFs were high. </br>
> 🟨 Which among MOFs had highest adsorption for Cd? ➡️ UiO-66-(COOH)<sub>4</sub> achieved slightly better results. </br>
> 🟨 Which among MOFs had the lowest adsorption for water? ➡️ UiO-66-(COOH)<sub>4</sub> consistently excluded the entry of water molecules.

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/3f794224-7353-4167-bc96-c42e494f7a25">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 5</strong>. Percent removal of Cd(II) atoms by UiO-66-(COOH), UiO-66-(COOH)<sub>2</sub>, UiO-66-(COOH)<sub>3</sub>, <br/> 
    and UiO-66-(COOH)<sub>4</sub> at different initial Cd(II) content: (a) 25 atoms, (b) 50 atoms, (c) 100 atoms, <br/> 
    and (d) 150 atoms.
</p>

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/1258490a-2e36-4652-b691-d6ceb5904bb0">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 6</strong>. Percent removal of water molecules by UiO-66-(COOH), UiO-66-(COOH)<sub>2</sub>, UiO-66-(COOH)<sub>3</sub>, <br/> 
    and UiO-66-(COOH)<sub>4</sub> at different initial Cd(II) content: (a) 25 atoms, (b) 50 atoms, (c) 100 atoms, <br/> 
    and (d) 150 atoms.
</p>

### B. Guest Molecule Distribution 

Further inspection of the behavior of Cd and water entry into the MOFs was conducted by preparing distribution heatmaps as shown in Fig. 7 and 8. The distribution of Cd(II) (Fig. 7) shows that the atoms penetrate to the center of all the MOFs. However, no clear trend was observed in the amount of Cd(II) atoms entering the MOF with the number of carboxylic acid substitutions on the BDC linkers. Meanwhile, the distribution of water molecules (Fig.8) indicates a decrease in water reaching the center of the MOFs from UiO-66-COOH to UiO-66-(COOH)<sub>4</sub>. The high concentration of water at the MOF edges suggests an attraction to the MOF region, though the pore size of the MOFs influences the extent of entry. The results suggest that Cd(II) penetration is not significantly influenced by the decreasing pore size from UiO-66-COOH to UiO-66-(COOH)<sub>4</sub>, which is likely due to its small ionic radius. In contrast, the observed reduction in water entry into the MOFs is likely attributed to the relatively larger molecular diameter (2.8 \AA) of water, which limits its ability to penetrate the narrower pores. 

> 🟨 Where are the Cd atoms located inside the MOFs? ➡️ Cd atoms penetrated all the way to the center of all the MOFs.
> 🟨 Where are the water atoms located inside the MOFs? ➡️ Water atoms penetrated all the way to the center of all the MOFs, but most are stuck at the MOF edges because of the larger size of water.

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/4d497791-bf1e-4e5c-a425-7e78cd2ef319">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 7</strong>. Heatmap showing the distribution of Cd(II) atoms within the simulation box where initial <br/> 
    Cd(II) count is 100 atoms. Dashed lines indicate the boundary between the empty region and <br/> 
    the MOF: (a) UiO-66-(COOH), (b) UiO-66-(COOH<sub>2</sub>, (c) UiO-66-(COOH)<sub>3</sub>, (d) UiO-66-(COOH)<sub>4</sub>
</p>


<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/100c6703-440a-447f-a2d3-0558fccb75b4">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 8</strong>. Heatmap showing the distribution of water atoms within the simulation box where initial <br/> 
    Cd(II) count is 100 atoms. Dashed lines indicate the boundary between the empty region and <br/> 
    the MOF: (a) UiO-66-(COOH), (b) UiO-66-(COOH<sub>2</sub>, (c) UiO-66-(COOH)<sub>3</sub>, (d) UiO-66-(COOH)<sub>4</sub>
</p>

### C. MOF Atom Preference

<p align="center" width="100%">
    <img width="60%" src="https://github.com/user-attachments/assets/f5347795-22cd-4001-812c-af8d54f2a0b4">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 9</strong>. Radial distribution function of Cd(II) around the framework atoms of (a) UiO-66-(COOH), (b) UiO-66-(COOH)<sub>2</sub>, <br/> 
    (c) UiO-66-(COOH)<sub>3</sub>, and (d) UiO-66-(COOH)<sub>4</sub> at initial Cd(II) content of 100 atoms. O1 and C1 pertain to oxygen <br/> 
    atoms of the metal nodes and to carbon atoms of the benzene linkers, respectively. O2 and C2 pertain to <br/> 
    the oxygen and carbon atoms of the substituted carboxylic groups.
</p>


<p align="center" width="100%">
    <img width="59.6%" src="https://github.com/user-attachments/assets/670ffb80-35cc-47b8-925a-9a1308a45f70">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 10</strong>.  Radial distribution function (left y-axis) of Cd(II) around oxygen atoms of substituted carboxylic <br/>
    groups of (a) UiO-66-(COOH), (b) UiO-66-(COOH<sub>2</sub>, (c) UiO-66-(COOH)<sub>3</sub>, and (d) UiO-66-(COOH)<sub>4</sub>  at initial <br/> 
    Cd(II) content of 100 atoms. O<sub>W</sub> and H<sub>W</sub> pertains to oxygen and hydrogen atoms of water, respectively.<br/> 
    Coordination number (right y-axis) of water with Cd(II) represented by blue dashed lines.
</p>
