# nonadiabatic-trajectory-analysis
These are the files used for my MSci research project, supervised by Rachel Crespo-Otero, at University College London.

Two conda environments were used in this project:
##### 1. `stcluster`
This environment is required to run the clustering and analysis code in this repository.

**Python version used:** 3.8.20 

To install the environment, run:

conda env create -f environment_stcluster.yml  
conda activate stcluster  

Once the environment is activated, install the required packages using:

pip install numpy pandas matplotlib scikit-learn scipy seaborn st-clustering

##### 2. `ulamdyn`
This environment is only required if you want to reproduce the raw input files from the original simulation outputs. To do this, install `ULaMDyn` and follow the procedure described in Ref. 22 of the report.

**Python version used:** 3.10.19

To install the environment, run:

conda env create -f environment_ulamdyn.yml  
conda activate ulamdyn  

Once the environment is activated, install the required packages using:

pip install ulamdyn numpy pandas scipy matplotlib h5py ase tqdm

## Notes
- The files in this repository are sufficient to run the main analysis workflow.
- Using the provided `.yml` files should reproduce the required Python versions automatically.
- Installing `ULaMDyn` is only necessary if you want to regenerate the raw processed files from the original trajectory data.
- Please contact me at `zccazw1@ucl.ac.uk` if you need further assistance with processing the files.
