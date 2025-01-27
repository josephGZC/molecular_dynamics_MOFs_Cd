![rec7B dat](https://github.com/user-attachments/assets/67dd1955-ea1a-44b9-80f4-68d788c08e5e)

# **Investigating the Removal of Cadmium from Water through UiO-66 Derivatives**

# Summary

### Problem
Cadmium Contamination in Water Sources

### Objectives 
* Determine the potential of UiO-66 and its derivatives as adsorbents of Cd. 
* Identify the best-performing UiO-66 derivative for Cd adsorption.
* Describe the adsorption mechanism. 

### Methods 
Simulate the following systems with cadmium and water:
* UiO-66
* UiO-66-(OH) 
* UiO-66-(COOH) 
* UiO-66-(COOH)<sub>2</sub> 
* UiO-66-(COOH)<sub>3</sub> 
* UiO-66-(COOH)<sub>4</sub>

### Insights
UiO-66 and its derivatives were able to remove at least 60% of cadmium from water, showing the potential of this MOF for Cd removal. 
UiO-66-(COOH)<sub>4</sub> removed 88% cadmium from water, which is why it is highly recommended to proceed to synthesis of this MOF for further testing
Cd interacts with the MOF via electrostatic interaction on the added oxygen atoms, which is why in functionalization, more oxygen atoms are favorable.

### Output
<img src="https://github.com/user-attachments/assets/2b105adf-f364-4152-8292-f7d1ae77f75c" width="15" height="15"> &nbsp; **Python Scripts**
* <a href="https://github.com/josephGZC/molecular_dynamics_MOFs_Cd/blob/main/plot-script_percent-removal/jup_rep_dyn_plots.ipynb" target="_blank">Percent Removal</a>
* <a href="https://github.com/josephGZC/molecular_dynamics_MOFs_Cd/blob/main/plot-script_heatmap-coordinate/jup_rep_heatmap.ipynb" target="_blank">Density Map</a>
* <a href="https://github.com/josephGZC/molecular_dynamics_MOFs_Cd/blob/main/plot-script_radial-distribution-function/jup_rep_rdf_plots.ipynb" target="_blank">Radial Distribution Function</a>

<img src="https://github.com/user-attachments/assets/126c7386-894b-4890-af87-775472fd30f7" width="15" height="15"> &nbsp; **Graph Preview**

<div style="overflow-x: auto; white-space: nowrap; padding: 10px; background-color: #f8f9fa; border-radius: 5px;"> <a href="https://github.com/user-attachments/assets/3be08deb-8fae-43bd-9d48-711d785f31c2" style="display: inline-block; margin-bottom: 10px;"> 
  <img src="https://github.com/user-attachments/assets/3be08deb-8fae-43bd-9d48-711d785f31c2" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 3"> </a> <a href="https://github.com/user-attachments/assets/eaeba421-311c-4059-9bff-c03796fe4c2e" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/eaeba421-311c-4059-9bff-c03796fe4c2e" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 4"> </a> <a href="https://github.com/user-attachments/assets/3f794224-7353-4167-bc96-c42e494f7a25" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/3f794224-7353-4167-bc96-c42e494f7a25" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 5"> </a> <a href="https://github.com/user-attachments/assets/1258490a-2e36-4652-b691-d6ceb5904bb0" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/1258490a-2e36-4652-b691-d6ceb5904bb0" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 6"> </a> <a href="https://github.com/user-attachments/assets/4d497791-bf1e-4e5c-a425-7e78cd2ef319" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/4d497791-bf1e-4e5c-a425-7e78cd2ef319" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 7"> </a> <a href="https://github.com/user-attachments/assets/100c6703-440a-447f-a2d3-0558fccb75b4" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/100c6703-440a-447f-a2d3-0558fccb75b4" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 8"> </a> <a href="https://github.com/user-attachments/assets/f5347795-22cd-4001-812c-af8d54f2a0b4" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/f5347795-22cd-4001-812c-af8d54f2a0b4" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 9"> </a> </div>
<p>
  <br>
</p>


# Technical Report

> Each section includes brief, symbol-marked sentences to help guide readers in understanding the problem variables and the questions being addressed. <br>
> <br>
> <img src="https://github.com/user-attachments/assets/970c2929-5c71-4213-9a77-416d7307e4e9" width="15" height="15"> &nbsp; for information <br>
> <img src="https://github.com/user-attachments/assets/104f5bba-400c-45a1-a1b1-19e9a223078a" width="15" height="15"> &nbsp; for procedural summaries <br>
> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; for analysis summaries

### Contents

<img src="https://github.com/user-attachments/assets/0bb79cc2-8c42-4829-b936-d93c6da8a132" width="15" height="15"> &nbsp; **Sections**
- [Background](#background)
- [Objectives](#objectives)
- [Simulation Setup](#simulation-setup)
- [Simulation Analysis](#simulation-analysis)
- [Conclusion](#conclusion)

## Background
[[back to contents](#contents)]

<p align="justify"> 
Cadmium contamination in water sources poses significant health and environmental risks, being linked to diseases like breast and lung cancer, bronchiolitis, and cerebral infection. Considering this, constant investigation on Cd(II) removal from water is essential. Among water purification techniques, adsorption is most promising due to its cost-effectiveness, mild operating conditions, and high efficiency. 
</p>
<p align="justify"> 
Metal-organic frameworks (MOFs) have emerged as promising adsorbents, offering high porosity, ultrahigh surface area, and customizable functionalities. <a href="https://doi.org/10.1021/ja8057953" target="_blank">UiO-66</a>, a Zr-based MOF with exceptional aqueous stability, has demonstrated significant potential in water treatment. Composed of Zr<sub>6</sub>O<sub>4</sub>(OH)<sub>4</sub> metal clusters connected by 1,4-benzedicarboxylic acid (BDC) linkers (<a href="#anchor-F1">Fig. 1</a>), UiO-66 exhibits a robust structure ideal for heavy metal adsorption. 
</p>

<a name="anchor-F1"></a>
<p align="center">
  <img src="https://github.com/user-attachments/assets/5dcf5770-a601-4791-964e-0efe4f0d04ca" width="70%" alt="Fig 1" style="margin-bottom: 0px;">
  <br>
  <span style="font-size: 80%;"><strong>Figure 1</strong>. The components (left) and unit cell (right) of UiO-66, where zirconium, oxygen, carbon, and hydrogen atoms are represented by blue, red, dark gray, and light gray spheres, respectively. The metal cluster Zr<sub>6</sub>O<sub>4</sub>(OH)<sub>4</sub> are represented by blue polyhedra. The tetrahedral and octahedral holes of UiO-66 are represented by pink and orange spheres, respectively.</span>
</p>

> <img src="https://github.com/user-attachments/assets/970c2929-5c71-4213-9a77-416d7307e4e9" width="15" height="15"> &nbsp; **Polymers are simply the combination of single chemical units.**
> * Carbohydrates are polymers of sugars.
> * DNA are polymers of nucleotides. 
> * MOFs are polymers of metals and organic compounds. 
> * UiO-66 (a MOF) is a polymer of Zr clusters and BDC linkers

## Objectives
[[back to contents](#contents)]

<p align="justify"> 
This study aims to evaluate cadmium adsorption performance of UiO-66 and its hydroxyl and carboxylic derivatives (UiO-66-(OH) and UiO-66-(COOH)) using molecular dynamics simulations, wherein the functional group attachment affects the local electron density of the MOFs and subsequent attraction with Cd. The research further seeks to analyze their adsorption mechanisms through distribution profiles, mobility analysis, radial distribution functions, and adsorption energy, providing insights into their viability for water purification applications.
</p>

> <img src="https://github.com/user-attachments/assets/104f5bba-400c-45a1-a1b1-19e9a223078a" width="15" height="15"> &nbsp;  **Listed Objectives** 
> 1. Determine the potential of UiO-66 and its derivatives as adsorbents of Cd. 
> 2. Identify the best-performing UiO-66 derivative for Cd adsorption.
> 3. Describe the adsorption mechanism. 

> <img src="https://github.com/user-attachments/assets/970c2929-5c71-4213-9a77-416d7307e4e9" width="15" height="15"> &nbsp; **Influence of interactions to be considered** 
> * More oxygen (O) → 
> * More negatively charged MOF → 
> * More attractive to postively charged cadmium (Cd) →
> * More Cd adsorption

> <img src="https://github.com/user-attachments/assets/970c2929-5c71-4213-9a77-416d7307e4e9" width="15" height="15"> &nbsp; **Influence of pore size to be considered** 
> * More carboxylic acid (COOH) → 
> * Bulkier linkers → 
> * Less pore size → 
> * Less entry of Cd

> <img src="https://github.com/user-attachments/assets/970c2929-5c71-4213-9a77-416d7307e4e9" width="15" height="15"> &nbsp; Increasing negatively charged atoms enhances favorable interactions but reduces pore size, highlighting the trade-off between electrostatic attraction and accessibility for optimal Cd adsorption.

## Simulation Setup
[[back to contents](#contents)]

<p align="justify"> 
UiO-66 and several of its derivatives where investigated. Specifically, UiO-66-(OH), UiO-66-(COOH), UiO-66-(COOH)<sub>2</sub>, UiO-66-(COOH)<sub>3</sub>, and UiO-66-(COOH)<sub>4</sub>. MOFs were positioned at the center of the simulation box as shown in <a href="#anchor-F2">Fig. 2</a>. A non-MOF region extends 20 Å from the negative and positive z-axes of the MOFs, which is referred to as the empty region.  For each MOF, four systems were packed with different Cd(II) number densities and equal number of water molecules.  Water molecules were randomly inserted throughout the entire system, while Cd(II) insertion was restricted to the empty region.
</p>

> <img src="https://github.com/user-attachments/assets/104f5bba-400c-45a1-a1b1-19e9a223078a" width="15" height="15"> &nbsp; The setup was prepared to answer the question, will Cd remain in water or will it go inside the MOFs?

<a name="anchor-F2"></a>
<p align="center">
  <img src="https://github.com/user-attachments/assets/ee0fb2d0-9840-480d-93a7-5a6e7d05bc9d" width="80%" alt="Fig 2" style="margin-bottom: 0px;">
  <br>
  <span style="font-size: 80%;"><strong>Figure 2</strong>. System snapshot showing UiO-66 packed with water (light blue sphere connected to white spheres) and Cd(II) (yellow spheres). In the MOF region, zirconium, oxygen, carbon, and hydrogen atoms are represented by blue, red, dark gray, and light gray spheres, respectively. The metal cluster nodes Zr<sub>6</sub>O<sub>4</sub>(OH)<sub>4</sub> are represented by blue polyhedra.</span>
</p>

> <img src="https://github.com/user-attachments/assets/104f5bba-400c-45a1-a1b1-19e9a223078a" width="15" height="15"> &nbsp; **MOFs investigated** 
> * UiO-66 
> * UiO-66-(OH) 
> * UiO-66-(COOH) 
> * UiO-66-(COOH)<sub>2</sub> 
> * UiO-66-(COOH)<sub>3</sub> 
> * UiO-66-(COOH)<sub>4</sub> 

## Simulation Analysis
[[back to contents](#contents)]

<p align="justify"> 
In analyzing the adsorption of the investigated MOFs, the <ins>performance of adosprtion</ins> and the <ins>mechanism of adsorption</ins> is explored. The performance was evaluated by counting the number of Cd atoms and water molecules found inside the MOFs, and subsequent calculation of  percent removal (i.e. percent of substance removed from the solution). A better-performing MOF correspond to adsorbing more Cd atoms (higher Cd percent removal) and adsoring less water molecules (lower water percent removal). Adsorption behavior was explored by looking into guest molecule (Cd or water) distribution and MOF atom preference (other analysis such as adsorption energy and mean square displacement were not included here). Several python scripts were created to analyze the trajectory output from the simulations. Pandas was used to process CSV files while seaborn was employed to generate plots. 
</p>

> <img src="https://github.com/user-attachments/assets/104f5bba-400c-45a1-a1b1-19e9a223078a" width="15" height="15"> &nbsp; **Analysis Flow Guide**
> * A. Determine adsorption performance from [Percent Removal](plot-script_percent-removal/jup_rep_dyn_plots.ipynb)
> * B. Determine guest molecule (Cd or Water) distribution [Density Map](plot-script_heatmap-coordinate/jup_rep_heatmap.ipynb)
> * C. Determine MOF atom interaction preference from [Radial Distribution Function](plot-script_radial-distribution-function/jup_rep_rdf_plots.ipynb) 

### A. Adsorption Performance

<p align="justify"> 
From all the simulations, the number of Cd(II) atoms within the MOF region and the empty region were plotted as a function of time as shown in <a href="#anchor-F3">Fig. 3</a> and <a href="#anchor-F4">Fig. 4</a>. This was presented for all MOFs across varying initial Cd(II) concentration. The results show that after an abrupt entry of Cd(II) into the MOF region within the 1-ns mark, further adsorption showed only minor fluctuations. In all cases, Cd(II) concentration remained consistently higher in the MOF region compared to the empty region until the simulation endpoint. These observations demonstrate that Cd(II) has an affinity for adsorption onto the MOFs, suggesting that their passage into the MOF is driven by more than just the initial concentration gradient.
</p>

> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; **Where the Cd atoms adsrobed to the MOFs?**
> * Yes, Cd atoms entered the MOFs and remained there until the end of the simulation.

<a name="anchor-F3"></a>
<p align="center">
  <img src="https://github.com/user-attachments/assets/3be08deb-8fae-43bd-9d48-711d785f31c2" width="80%" alt="Fig 3" style="margin-bottom: 0px;">
  <br>
  <span style="font-size: 80%;"><strong>Figure 3</strong>. Number of Cd(II) atoms adsorbed by UiO-66, UiO-66-OH, and UiO-66-COOH at different initial Cd(II) content. Specifically, the total initial count are (a-c) 100 and (d-f) 150 atoms.</span>
</p>

<a name="anchor-F4"></a>
<p align="center">
  <img src="https://github.com/user-attachments/assets/eaeba421-311c-4059-9bff-c03796fe4c2e" width="80%" alt="Fig 4" style="margin-bottom: 0px;">
  <br>
  <span style="font-size: 80%;"><strong>Figure 4</strong>. Number of Cd(II) atoms adsorbed by UiO-66-(COOH)<sub>2</sub>, UiO-66-(COOH)<sub>3</sub>, and UiO-66-(COOH)<sub>4</sub> at different initial Cd(II) content. Specifically, the total initial count are (a-c) 100 and (d-f) 150 atoms.</span>
</p>

<p align="justify"> 
When calculating percent removal in the system with initial Cd(II) atoms equal to 100, more than one MOF tied with the highest percent removal (<a href="#anchor-F5">Fig. 5</a>). In that series, UiO-66-(COOH)<sub>2</sub> and UiO-66-(COOH)<sub>4</sub> achieved slightly higher percent removal values compared to the other MOFs. UiO-66-(COOH)<sub>4</sub> achieved slightly higher percent removal in 25 and 150 initial Cd(II) content. The highest percent removal obtained for UiO-66-(COOH)<sub>4</sub> was 88%.
</p>
<p align="justify"> 
Besides percent removal of Cd(II), percent removal of water was also explored as shown in <a href="#anchor-F6">Fig. 6</a>. In this case, lower water adsorption is the desired outcome. Interestingly, while a distinct trend was not evident for Cd(II) percent removal across the incremental increase of carboxylic acid groups, a notable decrease in water adsorption was observed from UiO-66-(COOH) to UiO-66-(COOH)<sub>4</sub>. Given the significant difference in water percent removal across the investigated MOFs, UiO-66-(COOH)<sub>4</sub> is particularly effective at adsorbing Cd(II) while minimizing water uptake.
</p>

> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; **Are the MOFs suitable for Cd adsoprtion?**
> * Yes, becase Cd adsorption of all MOFs were high.

> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; **Which among MOFs had highest adsorption for Cd?**
> * UiO-66-(COOH)<sub>4</sub> achieved slightly better results.

> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; **Which among MOFs had the lowest adsorption for water?** 
> * UiO-66-(COOH)<sub>4</sub> consistently excluded the entry of water molecules.

<a name="anchor-F5"></a>
<p align="center">
  <img src="https://github.com/user-attachments/assets/3f794224-7353-4167-bc96-c42e494f7a25" width="80%" alt="Fig 5" style="margin-bottom: 0px;">
  <br>
  <span style="font-size: 80%;"><strong>Figure 5</strong>. Percent removal of Cd(II) atoms by UiO-66-(COOH), UiO-66-(COOH)<sub>2</sub>, UiO-66-(COOH)<sub>3</sub>, and UiO-66-(COOH)<sub>4</sub> at different initial Cd(II) content: (a) 25 atoms, (b) 50 atoms, (c) 100 atoms, and (d) 150 atoms.</span>
</p>

<a name="anchor-F6"></a>
<p align="center">
  <img src="https://github.com/user-attachments/assets/1258490a-2e36-4652-b691-d6ceb5904bb0" width="80%" alt="Fig 6" style="margin-bottom: 0px;">
  <br>
  <span style="font-size: 80%;"><strong>Figure 6</strong>. Percent removal of water molecules by UiO-66-(COOH), UiO-66-(COOH)<sub>2</sub>, UiO-66-(COOH)<sub>3</sub>, and UiO-66-(COOH)<sub>4</sub> at different initial Cd(II) content: (a) 25 atoms, (b) 50 atoms, (c) 100 atoms, and (d) 150 atoms.</span>
</p>

### B. Guest Molecule Distribution 

<p align="justify"> 
Further inspection of the behavior of Cd and water entry into the MOFs was conducted by preparing distribution heatmaps as shown in <a href="#anchor-F7">Fig. 7</a> and <a href="#anchor-F8">Fig. 8</a>. The distribution of Cd(II) (<a href="#anchor-F7">Fig. 7</a>) shows that the atoms penetrate to the center of all the MOFs. However, no clear trend was observed in the amount of Cd(II) atoms entering the MOF with the number of carboxylic acid substitutions on the BDC linkers. Meanwhile, the distribution of water molecules (<a href="#anchor-F8">Fig. 8</a>) indicates a decrease in water reaching the center of the MOFs from UiO-66-COOH to UiO-66-(COOH)<sub>4</sub>. The high concentration of water at the MOF edges suggests an attraction to the MOF region, though the pore size of the MOFs influences the extent of entry. The results suggest that Cd(II) penetration is not significantly influenced by the decreasing pore size from UiO-66-COOH to UiO-66-(COOH)<sub>4</sub>, which is likely due to its small ionic radius. In contrast, the observed reduction in water entry into the MOFs is likely attributed to the relatively larger molecular diameter (2.8 Å) of water, which limits its ability to penetrate the narrower pores. 
</p>

> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; **Where are the Cd atoms located inside the MOFs?** 
> * Cd atoms penetrated all the way to the center of all the MOFs. 

> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; **Where are the water atoms located inside the MOFs?**
> * Water atoms penetrated all the way to the center of all the MOFs, but most are stuck at the MOF edges because of the larger size of water.

<a name="anchor-F7"></a>
<p align="center">
  <img src="https://github.com/user-attachments/assets/4d497791-bf1e-4e5c-a425-7e78cd2ef319" width="80%" alt="Fig 7" style="margin-bottom: 0px;">
  <br>
  <span style="font-size: 80%;"><strong>Figure 7</strong>. Heatmap showing the distribution of Cd(II) atoms within the simulation box where initial Cd(II) count is 100 atoms. Dashed lines indicate the boundary between the empty region and the MOF: (a) UiO-66-(COOH), (b) UiO-66-(COOH<sub>2</sub>, (c) UiO-66-(COOH)<sub>3</sub>, (d) UiO-66-(COOH)<sub>4</sub>.</span>
</p>

<a name="anchor-F8"></a>
<p align="center">
  <img src="https://github.com/user-attachments/assets/100c6703-440a-447f-a2d3-0558fccb75b4" width="80%" alt="Fig 8" style="margin-bottom: 0px;">
  <br>
  <span style="font-size: 80%;"><strong>Figure 8</strong>. Heatmap showing the distribution of water atoms within the simulation box where initial Cd(II) count is 100 atoms. Dashed lines indicate the boundary between the empty region and the MOF: (a) UiO-66-(COOH), (b) UiO-66-(COOH<sub>2</sub>, (c) UiO-66-(COOH)<sub>3</sub>, (d) UiO-66-(COOH)<sub>4</sub>.</span>
</p>

### C. MOF Atom Interaction Preference

<p align="justify"> 
Radial distribution function of Cd(II) against all the carboxylic acid derivatives of UiO-66 were prepared as shown in <a href="#anchor-F9">Fig. 9</a>. Across all RDF plots, the closest peak appears around 1.7 Å, corresponding to the oxygen atoms in the carboxylic group (labeled O2 in <a href="#anchor-F9">Fig. 9</a>). This observation suggests that Cd(II) tends to remain in close proximity to this group, which indicates that electrostatic interaction between Cd(II) and oxygen atoms has significant contribution in the adsorption process. Cd(II) was also found to be within proximity of the oxygen atom in the metal nodes (represented as O1) but at a lower probability. This observation becomes less distinct with increasing carboxylic substitution as suggested by the gradual decrease of the blue and orange peaks in <a href="#anchor-F9">Fig. 9</a>, which further supports the preference of Cd(II) towards the oxygen atoms of the carboxylic groups in the BDC linkers.
</p>

> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; **Which atom of the MOF is Cd closest to?** 
> * Oxygen atoms of BDC linkers

> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; **What is the likely interaction between Cd and O?**
> * Close proximity of postively charged Cd to negatively charged O atoms suggest electrostatic itneraction.

<a name="anchor-F9"></a>
<p align="center">
  <img src="https://github.com/user-attachments/assets/f5347795-22cd-4001-812c-af8d54f2a0b4" width="80%" alt="Fig 9" style="margin-bottom: 0px;">
  <br>
  <span style="font-size: 80%;"><strong>Figure 9</strong>. Radial distribution function of Cd(II) around the framework atoms of (a) UiO-66-(COOH), (b) UiO-66-(COOH)<sub>2</sub>, (c) UiO-66-(COOH)<sub>3</sub>, and (d) UiO-66-(COOH)<sub>4</sub> at initial Cd(II) content of 100 atoms. O1 and C1 pertain to oxygen atoms of the metal nodes and to carbon atoms of the benzene linkers, respectively. O2 and C2 pertain to the oxygen and carbon atoms of the substituted carboxylic groups.</span>
</p>

## Conclusion
[[back to contents](#contents)]

<p align="justify"> 
Molecular dynamics simulations demonstrated the potential of UiO-66 derivatives as effective adsorbents for Cd(II) ions. When comparing the performance of the carboxylic derivatives of UiO-66, it was UiO-66-(COOH)<sub>4</sub> that achieved slightly better percent removal values. A more pronounced difference in performance was observed in the calculation of water percent removal. A clear trend emerged wherein water percent removal decreased as the number of carboxylic acid substituents increased. Thus, UiO-66-(COOH)<sub>4</sub> exhibited remarkable Cd(II) percent removal (up to 88%) while minimizing water uptake. Radial distribution functions revealed that the hydration of cadmium within MOFs plays a critical role in the adsorption process via hydrogen bonding. Additionally, the preference of Cd(II) towards electrostatic interaction with the oxygen atoms of the carboxylic acid substituent relay the importance of incorporating negatively charged groups to enhance MOF performance.
</p>
<p align="justify"> 
The findings of this study suggest that UiO-66-(COOH)<sub>4</sub> is a promising candidate for cadmium removal from water. The results also provide valuable insights into Cd(II) interactions with specific functional groups, which could inform future functionalization of metal-organic frameworks for water purification. To enhance the current investigation, it is recommended to simulate a range of metal pollutants to assess specificity across contaminants. Additionally, increasing the size of the MOF in simulations could accommodate a wider range of initial metal concentrations. Finally, laboratory synthesis and testing of UiO-66-(COOH)<sub>4</sub> would provide essential experimental validation of its removal efficiency.
</p>

<!-- This is commented out. 
<p align="center" width="100%">
    <img width="59.6%" src="https://github.com/user-attachments/assets/670ffb80-35cc-47b8-925a-9a1308a45f70">
</p>

<p align="center" style="font-size: 30%;">
    <strong>Figure 10</strong>.  Radial distribution function (left y-axis) of Cd(II) around oxygen atoms of substituted carboxylic <br/>
    groups of (a) UiO-66-(COOH), (b) UiO-66-(COOH<sub>2</sub>, (c) UiO-66-(COOH)<sub>3</sub>, and (d) UiO-66-(COOH)<sub>4</sub>  at initial <br/> 
    Cd(II) content of 100 atoms. O<sub>W</sub> and H<sub>W</sub> pertains to oxygen and hydrogen atoms of water, respectively.<br/> 
    Coordination number (right y-axis) of water with Cd(II) represented by blue dashed lines.
</p> 
-->
