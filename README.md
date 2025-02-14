# Scripts and Data for Bruns et al. (2022)

Script and data used to produce results in:  

- **Bruns, N. E., Heffernan, J. B., Ross, M. R. V., & Doyle, M. (2022).**  
  *A simple metric for predicting the timing of river phytoplankton blooms.*  
  Ecosphere, 13(12), e4348.  
  [https://doi.org/10.1002/ecs2.4348](https://doi.org/10.1002/ecs2.4348)

Both were published on Figshare:  

- **Bruns, N. (2022a).**  
  *Continuous Water Quality Data from Kansas River.* Figshare. Dataset.  
  [https://doi.org/10.6084/m9.figshare.21498588.v2](https://doi.org/10.6084/m9.figshare.21498588.v2)  

- **Bruns, N. (2022b).**  
  *Scripts for ‘Simple Metric for Predicting the Timing of River Phytoplankton Blooms’.* Figshare. Software.  
  [https://doi.org/10.6084/m9.figshare.21498582.v1](https://doi.org/10.6084/m9.figshare.21498582.v1)

---

## Repository Contents

- **`prepare_ms_data.Rmd`**  
  Script used to produce `gage_data_processed.RData` by obtaining and processing public USGS data.  

- **`make_ms_plots.Rmd`**  
  Script used to generate the manuscript figures.  

- **`gage_data_processed.RData`**  
  15-minute water quality and quantity measurements, including:
  - Chlorophyll-a (chl-a)
  - Nitrate (SUNA)
  - Turbidity
  - Temperature
  - Discharge  

  Data are from **four sites** along the mainstem of the Kansas River (USGS gage IDs: `"06887500"`, `06888990`, `"06892350"`, `"06892518"`).  

  This file is an **R list object** with four elements, each element is one wide-format table per site containing: 
  - **Columns**: Water quality parameters 
  - **Rows**: 15-minute measurements
