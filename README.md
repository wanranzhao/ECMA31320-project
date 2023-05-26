# ECMA31320-project
Final project for ECMA 31320 

## Research Topic

The effect of GVC participation rates on political instability 

## Data

Dependent: political instability 

Independent: GVC participation rates by industry sector; mixed, forward, and backward

IV: transport sector size; world-level GVC

Controls: 

1. GVC participation rates: from https://mrio.adbx.online/
   1. https://wits.worldbank.org/gvc/gvc-output-table.html
2. Controls: 
3. Dependent and IV: from our previous paper 

## File description

### [research proposal](https://github.com/wanranzhao/ECMA31320-project/blob/main/GVC%20and%20Political%20Stability%20-%20Research%20Proposal.docx)


### [`data`](https://github.com/wanranzhao/ECMA31320-project/tree/main/data) folder

#### [`GVC_data`](https://github.com/wanranzhao/ECMA31320-project/tree/main/data/GVC_data) folder

[`0.1 data_cleaning_gvc.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/GVC_data/0.1%20data_cleaning_gvc.ipynb): description to be written here

#### [`stability`](https://github.com/wanranzhao/ECMA31320-project/tree/main/data/stability) folder

[`0.2 political_stability_data_cleaning.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/stability/0.2%20political_stability_data_cleaning.ipynb): data cleaning code for political instability data

[`ASPO-Sample.dta`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/stability/ASPO-Sample.dta): political instability data

[`Comprehensive-Sample.dta`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/stability/Comprehensive-Sample.dta): political instability data

[`Read-me.pdf`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/stability/Read-me.pdf): political instability data codebook

[`stability_df.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/stability/stability_df.csv): cleaned political instability data

#### [`combined_data`](https://github.com/wanranzhao/ECMA31320-project/tree/main/data/combined_data) folder

[`0.3 Data_wrangling.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/combined_data/0.3%20Data_wrangling.ipynb): Data wrangling to merge the data from our 2 data sources and format them properly to be used in our models. 

[`outcome_and_control.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/combined_data/outcome_and_control.ipynb): code file to run analysis on initial data/variable selection. 

[`merged_052423.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/combined_data/merged_052423.csv): the merged WITS eora source gvc data with the stability data, this is our base panel data

[`gvcobp_data.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/combined_data/gvcobp_data.csv): merged and wrangled gvc backward data for use in analysis

[`gvcofp_data.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/combined_data/gvcofp_data.csv): merged and wrangled gvc forward data for use in analysis

[`gvcomix_data.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/combined_data/gvcomix_data.csv): merged and wrangled gvc mixed data for use in analysis



### [`code`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code) folder


#### [`External_IV`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/External_IV)

[`1.1_extIV_mix.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/1.1_extIV_mix.ipynb): Baseline 2SLS model regressions, using gvc mix participation data.

[`1.2_extIV_fp.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/1.2_extIV_fp.ipynb): Baseline 2SLS model regressions, using gvc forward participation data.

[`1.3_extIV_bp.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/1.3_extIV_bp.ipynb): Baseline 2SLS model regressions, using gvc backward participation data. Also includes data concatenation and robustness check.

[`1.4_robustness_checks.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/1.4_robustness_checks.ipynb): Robustness checks

[`bp_results.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/bp_results.csv): results for Baseline model gvc backward participation data

[`fp_results.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/fp_results.csv): results for Baseline model gvc backward participation data

[`mix_results.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/mix_results.csv): results for Baseline model gvc backward participation data

[`fuel_results.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/fuel_results.csv): Concatenated and filtered results for just the fuel sector, but all three gvc measures

#### [`Internal_IV`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/Internal_IV)

[`2_extIV_mix.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/Internal_IV/2_InternalIV.ipynb): All internal IV results, using (1) transport as external IV, (2) world-level GVC participation as external IV, and (3) no external IV. Results for gvc mixed, forward, and backward data are all inclued.


#### [`double_ml`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/double_ml)

[`3.1 ml-data-wrangling.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.1%20ml-data-wrangling.ipynb): data wrangling for double ml, as LATE identification needs binarized treatment and instrument.

[`3.2 ml-modeling-mix.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.2%20ml-modeling-mix.ipynb): double ml modeling on gvc mixed participation data. 

[`3.3 ml-modeling-forward.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.3%20ml-modeling-forward.ipynb): double ml modeling on gvc forward participation data. 

[`3.4 ml-modeling-backward.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.4%20ml-modeling-backward.ipynb): double ml modeling on gvc backward participation data. 

[`3.5 concat_results.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.5%20concat_results.ipynb): concatenated results for double ml.

[`df_mix.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/df_mix.csv): double ml gvc mixed participation data.

[`df_fp.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/df_fp.csv): double ml gvc forward participation data.

[`df_bp.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/df_bp.csv): double ml gvc backward participation data.

[`mix_res.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/mix_res.csv): double ml gvc mixed participation modeling results.

[`forward_res.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/forward_res.csv): double ml gvc forward participation modeling results.

[`backward_res.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/backward_res.csv): double ml gvc backward participation modeling results.


#### [`Plots`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/Plots)

[`4.1_plots.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/Plots/4.1_plots.ipynb): Code for ploting any graphs to use in the paper.

#### [`Summary_stat`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/Summary_stat)

[`5.1_summary.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/Plots/5.1_summary.ipynb): Code for summary stats (differentiated by variable onset2COWCS)

[`5.2_summary.Rmd`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/Plots/5.2_summary.Rmd): Code for summary stats (using stargazer packaged in R)

[`gvcobp_final_data.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/Summary_stat/gvcobp_final_data.csv): the same to [`gvcobp_data.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/combined_data/gvcobp_data.csv) after dropping NAs

[`gvcofp_final_data.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/Summary_stat/gvcofp_final_data.csv): the same to [`gvcofp_data.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/combined_data/gvcofp_data.csv) after dropping NAs

[`gvcomix_final_data.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/Summary_stat/gvcomix_final_data.csv): the same to [`gvcomix_data.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/data/combined_data/gvcomix_data.csv) after dropping NAs



### [`output`](https://github.com/wanranzhao/ECMA31320-project/tree/main/output) folder

#### [`Internal_IV`](https://github.com/wanranzhao/ECMA31320-project/tree/main/output/Internal_IV)

[`gvcomix`](https://github.com/wanranzhao/ECMA31320-project/blob/output/Internal_IV/gvcomix.txt): internal iv estimates for gvc mixed participation, without stationary controls

[`gvcofp`](https://github.com/wanranzhao/ECMA31320-project/blob/output/Internal_IV/gvcofp.txt): internal iv estimates for gvc forward participation, without stationary controls

[`gvcobp`](https://github.com/wanranzhao/ECMA31320-project/blob/output/Internal_IV/gvcobp.txt): internal iv estimates for gvc backward participation, without stationary controls

[`stationary_ctrlsgvcomix`](https://github.com/wanranzhao/ECMA31320-project/blob/output/Internal_IV/stationary_ctrlsgvcomix.txt): internal iv estimates for gvc mixed participation, with stationary controls

[`stationary_ctrlsgvcofp`](https://github.com/wanranzhao/ECMA31320-project/blob/output/Internal_IV/stationary_ctrlsgvcofp.txt): internal iv estimates for gvc forward participation, with stationary controls

[`stationary_ctrlsgvcobp`](https://github.com/wanranzhao/ECMA31320-project/blob/output/Internal_IV/stationary_ctrlsgvcobp.txt): internal iv estimates for gvc backward participation, with stationary controls 
