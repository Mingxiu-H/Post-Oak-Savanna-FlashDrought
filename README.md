# Flash Drought Dynamics and Impacts on Ecosystem Water Use Efficiency in the Post Oak Savanna

This repository contains the Google Earth Engine (GEE) scripts and Google Colab notebooks used for the study **“Flash drought dynamics and impacts on ecosystem water use efficiency in the Post Oak Savanna.”** The analysis covers the Post Oak Savanna (POS) ecoregion in Texas, USA, during 2000–2024.

The code supports the identification and characterization of flash drought events, analysis of ecosystem gross primary productivity (GPP), actual evapotranspiration (AET), and water use efficiency (WUE), and the additional analyses reported in the manuscript.

## Repository files

| File | Description |
| --- | --- |
| `GEE.txt` | **Main GEE code** used for the study's flash drought and ecosystem analyses. |
| `Flash_drought_v6_cleaned.ipynb` | **Main Google Colab notebook** used for subsequent data analysis and visualization. |
| `POS_rainfall.txt` | GEE code used to analyze precipitation conditions and provide rainfall background information for **2007 and 2011**. |
| `SA_POS_FD.txt` | GEE code used for the **sensitivity analysis** of flash drought results. |
| `Table2_statistical_analysis.ipynb` | Google Colab notebook used for the **statistical analysis underlying Table 2** of the manuscript. |

The `.txt` files contain JavaScript intended to be run in the Google Earth Engine Code Editor. The `.ipynb` files can be opened in Google Colab or another compatible Jupyter environment.

## Public datasets

The principal satellite datasets are available through the Google Earth Engine Data Catalog. All three MODIS products use **Collection 6.1**:

| Variable | MODIS product | GEE collection ID |
| --- | --- | --- |
| AET and potential evapotranspiration (PET) | MOD16A2GF | `MODIS/061/MOD16A2GF` |
| GPP | MOD17A2HGF | `MODIS/061/MOD17A2HGF` |
| Land cover | MCD12Q1 | `MODIS/061/MCD12Q1` |

Other inputs, including precipitation data and the POS study-area boundary, are referenced in the relevant scripts.

## How to use the code

1. Open `GEE.txt` in the [Google Earth Engine Code Editor](https://code.earthengine.google.com/). Review the study-area boundary and any custom asset paths, and replace inaccessible paths with assets available to your own GEE account. Run the relevant analysis and export any outputs needed for downstream processing.
2. Open `Flash_drought_v6_cleaned.ipynb` in [Google Colab](https://colab.research.google.com/). Update the input-file paths to point to your exported GEE outputs, then run the cells in the notebook's documented order.
3. Use `POS_rainfall.txt` for the supporting analysis of precipitation conditions in 2007 and 2011.
4. Use `SA_POS_FD.txt` for the flash drought sensitivity analysis.
5. Open `Table2_statistical_analysis.ipynb` to reproduce the statistical analysis associated with Table 2, using the corresponding input data.

The GEE scripts and notebooks may require access to intermediate outputs generated during the analysis. **Some GEE assets are user-created rather than public catalog datasets**; those assets must be made accessible or recreated before all steps can be rerun. Notebook input paths and package dependencies should be checked in the supplied code.

## Data and code availability

The publicly distributed MODIS datasets can be accessed directly through Google Earth Engine using the collection IDs above. This repository provides the analysis code; it does **not** include copies of the original MODIS datasets or a complete archive of all intermediate outputs.

## Citation

If you use this code, please cite the associated manuscript once its final publication details are available:

*Flash drought dynamics and impacts on ecosystem water use efficiency in the Post Oak Savanna.* Journal of Hydrology: Regional Studies. [Publication details to be added.]

## License

See the `LICENSE` file for the terms governing reuse of the code. If you choose to use the same **Creative Commons Attribution 4.0 International (CC BY 4.0)** license as your previous repository, add the corresponding license text to this repository. For a repository focused on software, a software-specific license such as MIT is also an option.
