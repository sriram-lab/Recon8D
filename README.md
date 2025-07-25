# Recon8D: A metabolic regulome network from oct-omics and machine learning
Recon8D utilizes eight omics classes (genomics (CNV and mutations), histone PTMs, DNA methylation, transcriptomics, RNA splicing, miRNA, lncRNA, proteomics, and phosphoproteomics) to predict metabolomic variation across cancer lines from the Cancer Cell Line Encyclopedia, thereby inferring a multiomic metabolic regulatory network. 

File descriptions

Recon8D_network.xlsx: Top 20 features for 225 RF metabolite models from 9 omics inputs along with confidence scores (0 through 8) based on the number of controls (out of 8 experiments) for which each feature appeared in the top 20.

ML_function.ipynb: ML script for random forests, XGBoost, ridge regression, and lasso regression, as well as feature importance generation. Includes example code for using histone PTM data as input. 

RF_results: Pearson's correlations and P values for all metabolite models from each of 8 omics classes. Significance is determined by Bonferroni-corrected P value. 

recon_mapping: MATLAB and Python scripts for extracting genes from reactions involving metabolites of interest and matching them with top feature lists, as well as a csv containing common gene name to BiggID translations. 

human_1_mapping.csv: List of metabolites from Recon3D with mapped Human1 IDs. 

example_datasets: metabolomics and histone PTM data that can be used to test the machine lerning code present in this repository. The rest of the CCLE data and trained models may be found here: https://doi.org/10.7303/syn68236153
