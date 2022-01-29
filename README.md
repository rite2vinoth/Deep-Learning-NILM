This project is submitted in partial fulfillment of MSc Data Science degree

Setup:
For running the notebook, it is required to install / setup NILMKTK from [here](https://github.com/nilmtk/nilmtk/blob/master/docs/manual/user_guide/install_user.md) and update the relevant files with the contents specified below

RunDisagg_Driver.ipynb - A driver notebook file which could be run to see the disaggregation algorithm in action.  

Contents:   

hybdisaggregator.py - Implementation of the proposed hybrid disaggregator based on GAN   
path: ../nilmtk/disaggregate   

metrics.py - Implementation of the evaluation criteria metrics.   
path: ../nilmtk.   

If there is an existing metrics.py please rename that file before placing the metrics.py file.  

UKDALE-HYB_bce-h1-washer dryer-45epochs.h5 - GAN Model of disaggregator   
path: ../
To be placed outside of nilmtk folder.   


The driver notebook can now be started and assuming the nilmtk installation worked correctly, the notebook can be run step by step.  

NOTE:  

1. The notebook also downloads a tar file [UKDale Dataset] (https://data.ukedc.rl.ac.uk/browse/edc/efficiency/residential/EnergyConsumption/Domestic/UK-DALE-2015/UK-DALE-disaggregated/ukdale.h5.tgz) containing the UKDALE dataset which is of substantial size. The code has a line to remove the TAR file once it has been extracted and only the h5 file is required.Users should note this disk space requirement. 

2. If there are any dependencies or packages that need to be installed, please install them within the conda environment you create to run this package.

3. Since there are several dependencies for nilmtk and because this is an old API some of the packages required may not be the latest versions. For these reasons, it is strongly recommended to install in a conda environment or a containerised environment like Docker. For the purposes of this project, focus was on analysis of the model rather than the packaging / production enablement of the model. 
