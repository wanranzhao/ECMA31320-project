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




### [`code`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code) folder

#### [`Summary_stat`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/Summary_stat)


#### [`Plots`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/Plots)

['4.1_plots.ipynb'](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/Plots/4.1_plots.ipynb): Code for ploting any graphs to use in the paper.


#### [`External_IV`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/External_IV)

['1.1_extIV_mix.ipynb'](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/1.1_extIV_mix.ipynb): Baseline 2SLS model regressions, using gvc mix participation data.

['1.2_extIV_fp.ipynb'](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/1.2_extIV_fp.ipynb): Baseline 2SLS model regressions, using gvc forward participation data.

['1.3_extIV_bp.ipynb'](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/1.3_extIV_bp.ipynb): Baseline 2SLS model regressions, using gvc backward participation data.

['bp_results.csv'](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/bp_results.csv): results for Baseline model gvc backward participation data

['fp_results.csv'](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/fp_results.csv): results for Baseline model gvc backward participation data

['mix_results.csv'](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/mix_results.csv): results for Baseline model gvc backward participation data

['fuel_results.csv'](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/External_IV/fuel_results.csv): Concatenated and filtered results for just the fuel sector, but all three gvc measures


#### [`Internal_IV`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/Internal_IV)


#### [`double_ml`](https://github.com/wanranzhao/ECMA31320-project/tree/main/code/double_ml)

[`3.1 ml-data-wrangling.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.1%20ml-data-wrangling.ipynb): data wrangling for double ml, as LATE identification needs binarized treatment and instrument.

[`3.2 ml-modeling-mix.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.2%20ml-modeling-mix.ipynb): double ml modeling on gvc mixed participation data. 

[`3.3 ml-modeling-forward.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.3%20ml-modeling-forward.ipynb): double ml modeling on gvc forward participation data. 

[`3.4 ml-modeling-backward.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.4%20ml-modeling-backward.ipynb): double ml modeling on gvc backward participation data. 

[`3.5 concat_results.ipynb`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/3.5%20concat_results.ipynb): concatenated results for double ml.

[`df_mix`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/df_mix.csv): double ml gvc mixed participation data.

[`df_fp.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/df_fp.csv): double ml gvc forward participation data.

[`df_bp.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/df_bp.csv): double ml gvc backward participation data.

[`mix_res.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/mix_res.csv): double ml gvc mixed participation modeling results.

[`forward_res.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/forward_res.csv): double ml gvc forward participation modeling results.

[`backward_res.csv`](https://github.com/wanranzhao/ECMA31320-project/blob/main/code/double_ml/backward_res.csv): double ml gvc backward participation modeling results.
