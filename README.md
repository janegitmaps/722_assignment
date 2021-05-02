README
722_assignment
Setup and installation

Required programs and accounts 
Please use the installation links and instructions provided below for Anaconda Navigator and USGS if required, otherwise collate your existing login credentials ready for input.

Anaconda Navigator program and login credentials.
https://docs.anaconda.com/anaconda/install/ for installation details consult the documentation in the link provided. Check the system requirements for your computer download the Anaconda installer and follow the installation wizard instructions. Create an account https://anaconda.org , open Anaconda Navigator and login.
USGS account and login credentials
Go to the USGS website and create a user account for access to satellite images from EarthExplorer. https://ers.cr.usgs.gov/login
GitHub account and repository link
https://github.com/join create username and password credentials, login to the github website before opening the repository link. The repository contains data required to run the scripts provided within the repository https://github.com/janegitmaps/722_assignment.git .


Creating the Anaconda Environment
Open Anaconda Prompt and run as an administrator, to call up a list of existing conda environments on your computer type conda env list in the command prompt. To create the new environment type conda create --name akumal python=3.6 specifying python=3.6 in this manner overrides the Anacondas automatic preference to install the newest python version available, it is also possible to install python3.5 in this manner. Next the new environment akumal needs to be activated conda activate akumal. Its important to activate the environment so that the modules installed in the next steps are installed to the newly created akumal environment. The active environment is listed in ( ) in first in the command prompt line (akumal) C:\WINDOWS\system32>  , once you have confirmed the active environment is akumal continue to module installation steps.
Add the modules individually, enter the first install instruction line, and follow the on screen proceed y/n prompt accordingly, before continuing to the next line which installs another module. 
conda install pandas 
conda install geopandas 
cona install notebook
conda install cartopy
conda install jupyter
conda install -c esri arcpy  
conda install -c jmcmurray os
conda install -c conda-forge rasterio
conda install -c conda-forge rioxarray
pip install landsatxplore
The landsatxlpore module is installed last as it uses pip for the installation, conda and pip do work together provided all conda environments are installed prior to any pip installations. Do note that if additional modules are later required then the environment needs to be recreated with conda module installations preceding all pip module installations. 

