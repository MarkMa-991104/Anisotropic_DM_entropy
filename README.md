# Anisotropic_DM_entropy

Improved Estimator of Dark Matter Entropy in Cosmological Simulations  
Master Research Project of Ke Ma  
submitted for  
MSci Theoretical Physics, Department of Physics and Astronomy, University College London  
supervised by  
Professor Andrew Pontzen  

# Pre-requisite

matplotlib  
numpy  
python  
pynbody (for installation instructions see https://pynbody.github.io/pynbody/)  

# Simulation outputs

My project used the pure dark matter cosmological simulation run by Lucie-Smith et al. (2018) produced from GADGET codes (Springel, 2005).  

Outputs of the simulation were 101 snapshots correspond to the same simulation at 101 different times.  

This github repository contains the final snapshot (snapshot_099) as well as its halo informations, placed in the folder "Simulation_Used".   

In order to run the codes (expect for "Time evolution.ipynb") in the folder "Codes-ipynb", one needs to download the contents inside the folder "Simulation_Used" and place them in the same directory with the codes.    

Note that the notebook "Time evolution.ipynb" requires snapshots_000, 009, 019, 029, 039, 049, 059, 069, 079 and 089 to run properly, which are not included in this github repository.  
 
# Codes for analysis

The codes and their functions are listed below:  

Halos-power law.ipynb   
To see the halo fitting result before the cutting-off inner and outer points.

Halos.ipynb  
To investigate the power law behaviour present in the radial entropy profile in Dark Matter halos, by fitting a linear function on the sample points of logQ against logr. 
3 halos was visualised, as well as their fitting results. The gamma value got from 51 halos was scatter-plotted and the mean was shown.

Large-scale.ipynb  
To invetigate the entropy distribution on large-scales, namely 100 Mpc in comoving coordinates. On the x-y plane of z=0 for present-day, 
The distribution of  Etropy per unit volume; Entropy per particle, for isotropic, anisotropic and difference; as well as density was plotted respectively.

Offset-Debugging.ipynb  
To solve/improve the offset problem encountered for the first algorithms. Displayed how normalisation procedure was constructed as well as the results on a test velocity distribution.

Time evolution.ipynb
To investigate the time evolution of entropy for 11 snapshots ranging from redshift~9 to the present day. Evolution of total entropy was plotted.
