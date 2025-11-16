# QualityModulation
The code is under review and will be available soon.

# Quick Start
- The project contains five core codes:
Code1-Dataset compilation.ipynb -> Corresponding to dataset augmentation and quality grouping.
Code2-Dataset statistics.ipynb -> Corresponding to Section 4.4 of the manuscript, including ASL and data volume display.
Code3-LIWC.ipynb -> Corresponding to the LIWC analysis process and plotting code.
Code4-Computational linguistic.ipynb -> Corresponds to manuscript Section 6.Includes linguistic error and toxicity patterns, dependent distance, and binary part-of-speech sequence analysis.
Code5-LLM zero-shot experiments.ipynb -> Contains a process for zero-shot experiments and error sample analysis.

- The 8 folders contained in the project are as follows:
[dic] is used to store the dictionary of liwc.
[fig] is where all the intended output images are saved.
[llms_pre] is the metric of all the recognition results of the LLM under the zero-shot prompt.
[MCFEND_CN] is the results of the RQ1a supplementary experiments.
[SUP_Gen_Q_Q] is the datasets of the RQ1a supplementary experiments.
[mcfend-based] Expected results of LIWC analysis of MCFEND.
[toutiao-based] Expected results of LIWC analysis of Toutiao.
[demo data of hanlp] Limited examples provided because the files are too large (1.85GB), involving Fig.10, Fig.11, Fig.D.1 and Fig.D.2.

- There are pkl, csv, and excel files, all of which are data used by the code.




# Main Instructions
- The sample file provided does not contain text that could be used to train harmful AI. All relevant data has been masked, which may result in some codes not achieving the desired effect.

- The following files involved in the code are too large (totaling 1.85GB), and only limited samples are provided: hanlp_data.csv, hanlp_data_lists.csv, hanlp_MCFEND.csv, hanlp_MCFEND_gen.csv, hanlp_MCFEND_gen_lists.csv, hanlp_MCFEND_lists.csv, hanlp_MCFEND_or.csv, hanlp_MCFEND_or_lists.csv;

- LIWC analysis raw results should be obtained on the requested dataset;

- Some code outputs process data that needs to be manually extracted and merged into xlsx, which is already detailed in the appropriate location.



# Main Dependencies
The code runs in the Python 3.10.13 environment in the format of Jupyter-recognizable ipynb. It contains the output that the code expects.
[pip install] is used to install dependencies：
numpy==1.24.4
pandas==2.0.3
matplotlib==3.6.2
scikit-learn==1.1.3
requests==2.31.0
scipy==1.12.0
seaborn==0.13.2
jieba==0.42.1
emoji==2.14.1
urllib3==1.26.15
hanlp==2.1.1
liwc==0.5.0




## File Structure Tree
├── 1_base_ks_test.xlsx
├── 1_dev_ks_test.xlsx
├── 1_hbd_ks_test.xlsx
├── 1_mcfned_ks_test.xlsx
├── 1_toutiao_ks_test.xlsx
├── all_quality_common_correct.pkl
├── all_quality_common_correct_M.pkl
├── all_quality_common_errors.pkl
├── all_quality_common_errors_M.pkl
├── asl_data.csv
├── asl_MCFEND_gen.csv
├── asl_MCFEND_or.csv
├── Code0-Dataset compilation.ipynb
├── Code1-Dataset statistics.ipynb
├── Code2-LIWC.ipynb
├── Code3-Computational linguistic.ipynb
├── Code4-LLM zero-shot experiments.ipynb
├── data_error_check.csv
├── dic
│   ├── sc_liwc.dic
│   └── toutiaobiaoqing.txt
├── diff_all.xlsx
├── diff_all_SUP.xlsx
├── diff_sd_all.xlsx
├── diff_sd_all_SUP.xlsx
├── fig
├── hanlp_data_lists.csv
├── hanlp_MCFEND_lists.csv
├── llms_pre
│   ├── all_aifk_llms_pre_mcfend.csv
│   ├── all_aifk_llms_pre_toutiao.csv
│   ├── all_llms_pre_mcfend.csv
│   ├── all_llms_pre_toutiao.csv
│   ├── average_llms_pre2_mcfend.csv
│   ├── average_llms_pre2_toutiao.csv
│   ├── average_llms_pre_mcfend.csv
│   ├── average_llms_pre_toutiao.csv
│   ├── goodall_aifk_llms_pre_toutiao.csv
│   ├── good_llms_pre2_mcfend.csv
│   ├── good_llms_pre2_toutiao.csv
│   ├── good_llms_pre_mcfend.csv
│   ├── good_llms_pre_toutiao.csv
│   ├── poor_llms_pre2_mcfend.csv
│   ├── poor_llms_pre2_toutiao.csv
│   ├── poor_llms_pre_mcfend.csv
│   └── poor_llms_pre_toutiao.csv
├── mcfend-based
│   ├── average_ks_stats_of_AIHM_FK.xlsx
│   ├── average_ks_stats_of_AIHM_RL.xlsx
│   ├── diff_average_AIHM_FK.xlsx
│   ├── diff_average_AIHM_RL.xlsx
│   ├── diff_good_AIHM_FK.xlsx
│   ├── diff_good_AIHM_RL.xlsx
│   ├── diff_poor_AIHM_FK.xlsx
│   ├── diff_poor_AIHM_RL.xlsx
│   ├── good_ks_stats_of_AIHM_FK.xlsx
│   ├── good_ks_stats_of_AIHM_RL.xlsx
│   ├── ks_stats_of_AIHM_FK.xlsx
│   ├── ks_stats_of_AIHM_RL.xlsx
│   ├── MSD_AI_FK_group.xlsx
│   ├── MSD_AI_RL_group.xlsx
│   ├── MSD_average_AI_FK_group.xlsx
│   ├── MSD_average_AI_RL_group.xlsx
│   ├── MSD_average_HM_FK_group.xlsx
│   ├── MSD_average_HM_RL_group.xlsx
│   ├── MSD_good_AI_FK_group.xlsx
│   ├── MSD_good_AI_RL_group.xlsx
│   ├── MSD_good_HM_FK_group.xlsx
│   ├── MSD_good_HM_RL_group.xlsx
│   ├── MSD_HM_FK_group.xlsx
│   ├── MSD_HM_RL_group.xlsx
│   ├── MSD_poor_AI_FK_group.xlsx
│   ├── MSD_poor_AI_RL_group.xlsx
│   ├── MSD_poor_HM_FK_group.xlsx
│   ├── MSD_poor_HM_RL_group.xlsx
│   ├── poor_ks_stats_of_AIHM_FK.xlsx
│   └── poor_ks_stats_of_AIHM_RL.xlsx
├── mcfend_5387_real_for_CheapAI_Processed.csv
├── mcfend_9339_Fake_for_CheapFake_Processed.csv
├── MCFEND_CN
│   ├── ALL
│   │   ├── 0_ks_stats_of_base_AIHM_FK.xlsx
│   │   ├── 0_ks_stats_of_base_AIHM_RL.xlsx
│   │   ├── 0_ks_stats_of_dev_AIHM_FK.xlsx
│   │   ├── 0_ks_stats_of_dev_AIHM_RL.xlsx
│   │   ├── 0_ks_stats_of_hbd_AIHM_FK.xlsx
│   │   ├── 0_ks_stats_of_hbd_AIHM_RL.xlsx
│   │   ├── diff_base_AIHM_FK.xlsx
│   │   ├── diff_base_AIHM_RL.xlsx
│   │   ├── diff_dev_AIHM_FK.xlsx
│   │   ├── diff_dev_AIHM_RL.xlsx
│   │   ├── diff_hbd_AIHM_FK.xlsx
│   │   ├── diff_hbd_AIHM_RL.xlsx
│   │   ├── MSD_base_AI_FK_group.xlsx
│   │   ├── MSD_base_AI_RL_group.xlsx
│   │   ├── MSD_base_HM_FK_group.xlsx
│   │   ├── MSD_base_HM_RL_group.xlsx
│   │   ├── MSD_dev_AI_FK_group.xlsx
│   │   ├── MSD_dev_AI_RL_group.xlsx
│   │   ├── MSD_dev_HM_FK_group.xlsx
│   │   ├── MSD_dev_HM_RL_group.xlsx
│   │   ├── MSD_hbd_AI_FK_group.xlsx
│   │   ├── MSD_hbd_AI_RL_group.xlsx
│   │   ├── MSD_hbd_HM_FK_group.xlsx
│   │   └── MSD_hbd_HM_RL_group.xlsx
│   ├── average_ks_stats_of_base_AIHM_FK.xlsx
│   ├── average_ks_stats_of_base_AIHM_RL.xlsx
│   ├── average_ks_stats_of_dev_AIHM_FK.xlsx
│   ├── average_ks_stats_of_dev_AIHM_RL.xlsx
│   ├── average_ks_stats_of_hbd_AIHM_FK.xlsx
│   ├── average_ks_stats_of_hbd_AIHM_RL.xlsx
│   ├── diff_base_average_AIHM_FK.xlsx
│   ├── diff_base_average_AIHM_RL.xlsx
│   ├── diff_base_good_AIHM_FK.xlsx
│   ├── diff_base_good_AIHM_RL.xlsx
│   ├── diff_base_poor_AIHM_FK.xlsx
│   ├── diff_base_poor_AIHM_RL.xlsx
│   ├── diff_dev_average_AIHM_FK.xlsx
│   ├── diff_dev_average_AIHM_RL.xlsx
│   ├── diff_dev_good_AIHM_FK.xlsx
│   ├── diff_dev_good_AIHM_RL.xlsx
│   ├── diff_dev_poor_AIHM_FK.xlsx
│   ├── diff_dev_poor_AIHM_RL.xlsx
│   ├── diff_hbd_average_AIHM_FK.xlsx
│   ├── diff_hbd_average_AIHM_RL.xlsx
│   ├── diff_hbd_good_AIHM_FK.xlsx
│   ├── diff_hbd_good_AIHM_RL.xlsx
│   ├── diff_hbd_poor_AIHM_FK.xlsx
│   ├── diff_hbd_poor_AIHM_RL.xlsx
│   ├── good_ks_stats_of_base_AIHM_FK.xlsx
│   ├── good_ks_stats_of_base_AIHM_RL.xlsx
│   ├── good_ks_stats_of_dev_AIHM_FK.xlsx
│   ├── good_ks_stats_of_dev_AIHM_RL.xlsx
│   ├── good_ks_stats_of_hbd_AIHM_FK.xlsx
│   ├── good_ks_stats_of_hbd_AIHM_RL.xlsx
│   ├── MSD_base_average_AI_FK_group.xlsx
│   ├── MSD_base_average_AI_RL_group.xlsx
│   ├── MSD_base_good_AI_FK_group.xlsx
│   ├── MSD_base_good_AI_RL_group.xlsx
│   ├── MSD_base_poor_AI_FK_group.xlsx
│   ├── MSD_base_poor_AI_RL_group.xlsx
│   ├── MSD_dev_average_AI_FK_group.xlsx
│   ├── MSD_dev_average_AI_RL_group.xlsx
│   ├── MSD_dev_good_AI_FK_group.xlsx
│   ├── MSD_dev_good_AI_RL_group.xlsx
│   ├── MSD_dev_poor_AI_FK_group.xlsx
│   ├── MSD_dev_poor_AI_RL_group.xlsx
│   ├── MSD_hbd_average_AI_FK_group.xlsx
│   ├── MSD_hbd_average_AI_RL_group.xlsx
│   ├── MSD_hbd_good_AI_FK_group.xlsx
│   ├── MSD_hbd_good_AI_RL_group.xlsx
│   ├── MSD_hbd_poor_AI_FK_group.xlsx
│   ├── MSD_hbd_poor_AI_RL_group.xlsx
│   ├── poor_ks_stats_of_base_AIHM_FK.xlsx
│   ├── poor_ks_stats_of_base_AIHM_RL.xlsx
│   ├── poor_ks_stats_of_dev_AIHM_FK.xlsx
│   ├── poor_ks_stats_of_dev_AIHM_RL.xlsx
│   ├── poor_ks_stats_of_hbd_AIHM_FK.xlsx
│   └── poor_ks_stats_of_hbd_AIHM_RL.xlsx
├── mcfend_error_check.csv
├── MCFEND_for_classification.csv
├── merge_22075_with_all_model.csv
├── README.md
├── SUP_Gen_Q_Q
│   ├── Q_Q_【base_fake_ok】mcfend_9466_Fake_for_CheapFeak_base.csv
│   ├── Q_Q_【base_real_ok】mcfend_5395_real_for_CheapAI_base.csv
│   ├── Q_Q_【de_fake_ok】mcfend_8794_Fake_for_CheapFeak_de.csv
│   ├── Q_Q_【de_real_ok】mcfend_5255_real_for_CheapAI_de.csv
│   ├── Q_Q_【hb_fake_ok】mcfend_5743_Fake_for_CheapFeak_hb.csv
│   ├── Q_Q_【hb_real_ok】mcfend_3440_real_for_CheapAI_hb.csv
│   ├── 【all】mcfend_base.csv
│   ├── 【all】mcfend_dev.csv
│   └── 【all】mcfend_hbd.csv
├── Table2-ALL-LIWC.xlsx
├── TableE1-ALL-LIWC.xlsx
└── toutiao-based
    ├── average_ks_stats_of_AIHM_FK.xlsx
    ├── average_ks_stats_of_AIHM_RL.xlsx
    ├── diff_AIHM_FK.xlsx
    ├── diff_AIHM_RL.xlsx
    ├── diff_average_AIHM_FK.xlsx
    ├── diff_average_AIHM_RL.xlsx
    ├── diff_good_AIHM_FK.xlsx
    ├── diff_good_AIHM_RL.xlsx
    ├── diff_poor_AIHM_FK.xlsx
    ├── diff_poor_AIHM_RL.xlsx
    ├── good_ks_stats_of_AIHM_FK.xlsx
    ├── good_ks_stats_of_AIHM_RL.xlsx
    ├── ks_stats_of_AIHM_FK.xlsx
    ├── ks_stats_of_AIHM_RL.xlsx
    ├── MSD_AI_FK_group.xlsx
    ├── MSD_AI_RL_group.xlsx
    ├── MSD_average_AI_FK_group.xlsx
    ├── MSD_average_AI_RL_group.xlsx
    ├── MSD_average_HM_FK_group.xlsx
    ├── MSD_average_HM_RL_group.xlsx
    ├── MSD_good_AI_FK_group.xlsx
    ├── MSD_good_AI_RL_group.xlsx
    ├── MSD_good_HM_FK_group.xlsx
    ├── MSD_good_HM_RL_group.xlsx
    ├── MSD_HM_FK_group.xlsx
    ├── MSD_HM_RL_group.xlsx
    ├── MSD_poor_AI_FK_group.xlsx
    ├── MSD_poor_AI_RL_group.xlsx
    ├── MSD_poor_HM_FK_group.xlsx
    ├── MSD_poor_HM_RL_group.xlsx
    ├── poor_ks_stats_of_AIHM_FK.xlsx
    └── poor_ks_stats_of_AIHM_RL.xlsx
