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


