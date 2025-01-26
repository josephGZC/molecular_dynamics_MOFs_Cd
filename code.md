![rec7B dat](https://github.com/user-attachments/assets/67dd1955-ea1a-44b9-80f4-68d788c08e5e)

# **Investigating the Removal of Cadmium from Water through UiO-66 Derivatives**

> Each section includes brief, symbol-marked sentences to help guide readers in understanding the problem variables and the questions being addressed. <br>
> <br>
> <img src="https://github.com/user-attachments/assets/970c2929-5c71-4213-9a77-416d7307e4e9" width="15" height="15"> &nbsp; for information <br>
> <img src="https://github.com/user-attachments/assets/104f5bba-400c-45a1-a1b1-19e9a223078a" width="15" height="15"> &nbsp; for procedural summaries <br>
> <img src="https://github.com/user-attachments/assets/7a87286b-2c51-44e7-8ed2-ce709c7837ad" width="15" height="15"> &nbsp; for analysis summaries

### Contents

<img src="https://github.com/user-attachments/assets/0bb79cc2-8c42-4829-b936-d93c6da8a132" width="15" height="15"> &nbsp; **Sections**
- [Overview](#overview)
- [Objectives](#objectives)
- [Simulation Setup](#simulation-setup)
- [Simulation Analysis](#simulation-analysis)
- [Conclusion](#conclusion)
  
<img src="https://github.com/user-attachments/assets/2b105adf-f364-4152-8292-f7d1ae77f75c" width="15" height="15"> &nbsp; **Python Scripts**
* <a href="https://github.com/josephGZC/molecular_dynamics_MOFs_Cd/blob/main/plot-script_percent-removal/jup_rep_dyn_plots.ipynb" target="_blank">Percent Removal</a>
* <a href="https://github.com/josephGZC/molecular_dynamics_MOFs_Cd/blob/main/plot-script_heatmap-coordinate/jup_rep_heatmap.ipynb" target="_blank">Density Map</a>
* <a href="https://github.com/josephGZC/molecular_dynamics_MOFs_Cd/blob/main/plot-script_radial-distribution-function/jup_rep_rdf_plots.ipynb" target="_blank">Radial Distribution Function</a>

<img src="https://github.com/user-attachments/assets/126c7386-894b-4890-af87-775472fd30f7" width="15" height="15"> &nbsp; **Graph Preview**

Here’s an early preview of the selected images:

<div style="overflow-x: auto; white-space: nowrap; padding: 10px; background-color: #f8f9fa; border-radius: 5px;"> <a href="https://github.com/user-attachments/assets/3be08deb-8fae-43bd-9d48-711d785f31c2" style="display: inline-block; margin-bottom: 10px;"> 
  <img src="https://github.com/user-attachments/assets/3be08deb-8fae-43bd-9d48-711d785f31c2" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 3"> </a> <a href="https://github.com/user-attachments/assets/eaeba421-311c-4059-9bff-c03796fe4c2e" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/eaeba421-311c-4059-9bff-c03796fe4c2e" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 4"> </a> <a href="https://github.com/user-attachments/assets/3f794224-7353-4167-bc96-c42e494f7a25" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/3f794224-7353-4167-bc96-c42e494f7a25" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 5"> </a> <a href="https://github.com/user-attachments/assets/1258490a-2e36-4652-b691-d6ceb5904bb0" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/1258490a-2e36-4652-b691-d6ceb5904bb0" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 6"> </a> <a href="https://github.com/user-attachments/assets/4d497791-bf1e-4e5c-a425-7e78cd2ef319" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/4d497791-bf1e-4e5c-a425-7e78cd2ef319" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 7"> </a> <a href="https://github.com/user-attachments/assets/100c6703-440a-447f-a2d3-0558fccb75b4" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/100c6703-440a-447f-a2d3-0558fccb75b4" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 8"> </a> <a href="https://github.com/user-attachments/assets/f5347795-22cd-4001-812c-af8d54f2a0b4" style="display: inline-block; margin-bottom: 10px;"> <img src="https://github.com/user-attachments/assets/f5347795-22cd-4001-812c-af8d54f2a0b4" width="150" height="100" style="border-radius:10px; box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);" alt="Fig 9"> </a> </div>
<p>
  <br>
</p>


How are clusters identified in the simulation?

Fortran is used to identify clusters while python is used for further post processing.
