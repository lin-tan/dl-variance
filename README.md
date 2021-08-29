# Problems and Opportunities in Training Deep Learning Software Systems: An Analysis of Variance

This is the artifact repository for the ASE 2020 paper [Problems and Opportunities in Training Deep Learning Software Systems: An Analysis of Variance](https://conf.researchr.org/details/ase-2020/ase-2020-papers/13/Problems-and-Opportunities-in-Training-Deep-Learning-Software-Systems-An-Analysis-of)

## Artifacts list:

File |Description
---|---
[Survey.Questions.pdf](https://github.com/lin-tan/dl-variance/releases/download/1.0/Survey.Questions.pdf) | The survey questions
[Survey.Report.pdf](https://github.com/lin-tan/dl-variance/releases/download/1.0/Survey.Report.pdf) | The survey aggregated report
[Training configuration.pdf](https://github.com/lin-tan/dl-variance/releases/download/1.0/Training.configuration.pdf) | The training configuration for the 6 networks
[Relevant-AI-Papers.csv](https://github.com/lin-tan/dl-variance/releases/download/1.0/Relevant-AI-Papers.csv) | The list of relevant AI papers in our survey
[Relevant-Non-AI-Papers.csv](https://github.com/lin-tan/dl-variance/releases/download/1.0/Relevant-Non-AI-Papers.csv) |The list of relevant Non-AI papers in our survey
[analysis_result.csv](https://github.com/lin-tan/dl-variance/releases/download/1.0/analysis_result.csv) | The analysis result for our experiments
[analysis_raw.csv](https://github.com/lin-tan/dl-variance/releases/download/1.0/analysis_raw.csv) | The raw analysis result for our experiments
[weights.tar.gz](https://github.com/lin-tan/dl-variance/releases/download/1.0/weights.tar.gz) | The folder containing the weights of the most extreme models in our experiments


## Details of the paper listing files:

**Relevant-AI-Papers.csv**
This file contains the list of AI papers that we found relevant to our study during our paper survey.

**Relevant-Non-AI-Papers.csv**
This file contains the list of Non-AI papers that we found relevant to our study during our paper survey.

Column| Description
---|---
Conference| The conference
Title| Paper title
Relevant to our study? | Does the work train deep learning networks?
Do they do multiple identical runs? | Does the work report multiple identical runs?

## Details of the analysis files:
**analysis_result.csv**
This file contains the main analysis result of the experimental runs

Column| Description
---|---
backend| core library
backend_version| core library version
cuda_version| cuda version
cudnn_version| cudnn version
network| network	
random_seed	| if 1 ->  fixed-seed, if -1 -> random seed
stopping_type| selection criterion	
no_try| number of identical runs	
max_accuracy_diff|	largest overall accuracy difference
max_accuracy| overall accuracy of the most accurate run	
min_accuracy| overall accuracy of the least accurate run	
std_dev_accuracy| overall accuracy standard deviation	
mean_accuracy| mean overall accuracy	
max_diff_label| the class index with the largest accuracy gap for this experimental set	
max_per_label_acc_diff| largest per-class accuracy difference	
max_label_accuracy	| largest per-class accuracy for the class 
min_label_accuracy| lowest per-class accuracy for the class	
no_samples_max_diff| number of test samples for class (max_diff_label)	
max_std_label| the class index with the largest per-class accuracy standard deviation for this experimental set		
max_per_label_acc_std| the per-class accuracy standard deviations	
no_samples_max_std| number of test samples for class (max_std_label)	
max_convergent_diff| largest convergence time difference	
max_convergent| convergence time of the slowest run (most time)	
min_convergent| convergence time of the fastest run (least time)	
std_dev_convergent	| standard deviation of convergence times
mean_convergent| average convergence time	
max_convergent_diff_epoch| largest gap of the number of epochs to convergence 	
max_convergent_epoch| largest number of epochs to convergence	
min_convergent_epoch| smallest number of epochs to convergence	
std_dev_convergent_epoch| standard deviation of the number of epochs to convergence
mean_convergent_epoch| average number of epochs to convergence

**analysis_raw.csv**
This file contains the overall accuracy of all training runs

Column| Description
---|---
backend| core library
backend_version| core library version
cuda_version| cuda version
cudnn_version| cudnn version
network| network	
random_seed	| if 1 ->  fixed-seed, if -1 -> random seed
stopping_type| selection criterion	
try| run index
accuracy| overall accuracy of the model
convergent| time to convergence of this run
convergent_epoch| number of epochs to convergence

*This survey study has been reviewed and qualifies for an exemption under 45 CFR 46.101(b)(2) from Purdue's Institutional Review Board (IRB-2020-234).*

