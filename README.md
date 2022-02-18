# A Comparison of Remotely Sensed Environmental Predictors for Avian Distributions
Code for [Hopkins et al., 2022. Landscape Ecology]<br /> 
https://doi.org/10.1007/s10980-022-01406-y
***

1. Download the data and save it in your working directory.: https://figshare.com/projects/A_Comparison_of_Remotely_Sensed_Environmental_Predictors_for_Avian_Distributions/94619. 

2. Generate SDMs (RF models) and thier predictions. <br /><br /> **Run ```run_model.R```**
<br /><br /> Create a new "results" folder in your working directory. Withing the "results" folder, create a folder for each model and within each model, create folders for each species. The path should look like: ```<working_directory>\\<model>\\<species>```. Moeve the .RData test table(s) created by run_model.R to the associated folder(s).

4. Evaluate models by comparing AUCs across species and spectral predictor sets. <br /><br /> **Run ```evaluation.R```** 

5. Identifiy which spectral predictor sets performed best across the entire set of species and compare all pairs of spectral predictor sets with Nemenyi post-hoc analysis. <br /><br /> **Run ```statistical_analysis.R```** 

6. (Optional) Generate plots. <br /><br /> **Run ```publication_plots.R```** 
