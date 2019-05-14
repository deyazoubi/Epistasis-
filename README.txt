
##################empirical data############
#all data used in this paper are taken from {Szappanos,2011}

for both data files we exclude essential genes and genes associated with blocked reactions  
and then calculated epistasis

combined_data_highconfidence.txt  is used for Epistasis analysis 

sgadata_metabolic_array_Deya.txt is used for is used for synthetic lethal analysis 


################## model##################
 - growth medium was set up to mimic the one used in the experiment 
 - 5 genes were deleted to mimic the strain background used in the experiments.

#Rdata files with the yeast7.6  model

##################kcat+molecular weights##################

experimental kcat values for 535 enzymes and molecular weights are taken from {Desouki, 2016}
for the remaining enzymes, we use the median of the 535 known values
for more detailed informations please see CRAN Package sybilccFBA
https://cran.r-project.org/web/packages/sybilccFBA/index.html

##################Results[Raw data]##################

Epistasis.Rdata:Rdata file with a Epistasis result at different constraint based method
dfs_neg1.Rdata:Rdata file with a recall, FPrate, precision, cutoffs, TP ,FP,  FN, TN,  result for negative interaction at different constraint based method 
 
dfs_pos1.Rdata:Rdata file with a recall, FPrate, precision, cutoffs, TP ,FP,  FN, TN,  result for positive interaction at different constraint based method 
##################synthetic lethal Results[Raw data]##################
SL_CBM.Rdata:Rdata file with a synthetic lethal result at different constraint based method
the results contain
ORF1    ORF2  WxWy(product of single mutant fitness)   Wxy(double mutant fitness)   Σ(Epistasis score simulation) EP.exp(Epistasis score experiment ) DMF.exp(double mutant fitness experiment) 
