# List-of-Projects
## Genomics and machine learning
### 1. Identifying the context of mutations in a cancer genome
Exploring the genomic context of cancer-causing mutations and using that to differentiate between driver and passenger mutations is not very well 
explored. In this study, we use both publicly available cancer mutation data from the [COSMIC v90](https://cancer.sanger.ac.uk/cosmic) and
WGS data from isogenic mice models affected with PDAC to extract sequence-based features from the neighbourhood of a mutation. 
Our goal is to develop novel algorithms that apply methods from Natural Language Processing and machine learning to analyse the sequence and positional 
context of genomic mutations to distinguish between driver and passengers.  

**Supervisors**: [Dr Karthik Raman](https://home.iitm.ac.in/kraman/lab/karthik/) and [Dr Balaraman Ravindran](https://www.cse.iitm.ac.in/~ravi/)  
**Category:** Masters project  
**Report:** A [brief analysis](https://docs.google.com/document/d/13MOsX7WKgRlUIp4-PJP8s5HroQTX2DOOf2WrI2T--vY/edit?usp=sharing) of the results obtained so far.  
**Poster:** [Link](https://drive.google.com/file/d/1dQzLGUdUOzta6rBrqoZCl7wE5Wlj2Qi2/view?usp=sharing)
  
  

### 2. Integrating genomic and clinical data to differentiate between sepsis patients having complicated course outcomes
Sepsis is a life threatning condition and an estimated 4.2 million newborns and children are affected every year. In the first part of this project we analyzed publicly available pediatric sepsis gene expression data [GSE66099](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE66099) to differentiate between survivors and non-survivors. Complicated course outcomes is defined as mortality by 28 days or persistence of greater than or equal to two organ failures at day 7 of septic shock. Using the complicated course labels provided by our [collaborators](https://www.cincinnatichildrens.org/bio/w/hector-wong), we did differential gene expression analysis on the same microarray data. The differentially expressed genes (DEGs) or the biomarkers found in this analysis were validated using already existing studies and functional analysis was also performed. Next, using the same microarray data, we experimented with different feature selection approaches and extracted a set of stable features (genes) for building machine learning models for classifying complicated course vs uncomplicated course patients.  

**Supervisors**: [Dr Rishikesan Kamaleswaran](https://www.kamaleswaran.com/), [Dr Akram Mohammed](https://akram-mohammed.github.io/)  
**Category:** [Google Summer of Code](https://summerofcode.withgoogle.com/organizations/5759105409482752/#5859209076277248) project.     
**Slides:** [Link](https://drive.google.com/file/d/12hzYFZTlAtSFICj8AqjTwiGq6gXrfrT_/view?usp=sharing)  
**Initial proposal:** [Proposal](https://github.com/banerjeeshayantan/GSOC-complicated_Course_project/blob/master/GSOC-proposal.pdf)    
**Repository:** [Github repo containing the final report and codes](https://github.com/banerjeeshayantan/GSOC-complicated_Course_project).  
**Funding agency:** [Google](https://developers.google.com/open-source/gsoc/help/student-stipends)  


### 3. Integrative analysis and identification of cancer driver genes using publicly available mutation data
Driver mutations are somatic mutations that help in cancer progression while passenger mutations have no effect on the fitness of a cancer cell. Distinguising drivers from passengers is challenging because drivers occur less frequently than passengers and their functional impact is not intuitively obvious. Several computational approaches have been developed so far to generate a list of high confidence cancer driver genes. In this project, three of the most popular driver prediction tools were used to identify driver genes across six cancer types and their accuracy in terms of overlap with the [Cancer Gene Census](https://cancer.sanger.ac.uk/census) were noted. Mutational load comparison between the downloaded mutation data and TCGA cohorts was performed and a list of common oncogenic pathways affected for each cancer type were validated with the existing literature. Finally, a list of high confidence drivers predicted by all three tools were generated. A short analysis showed that different cancer types share altered genetic components that can be used as prime therapeutic targets.   
**Category:** Independent research project   
**Repository:** [Link](https://github.com/banerjeeshayantan/Driver_gene_identificantion)  
**Detailed write-up:** [Link](https://docs.google.com/document/d/1VCLoe-IbIr_CIarEAcDNW3Z9O31Z1KcpNVPpA1Be8_w/edit?usp=sharing)  
 
 ### 4. Classifying cancerous tissue using gene expression data  
DNA microarray technology is used to measure the expression levels of genes under various conditions. Differential expression of these genes can elucidate newer insights into the functioning of various diseases. Usually, microarray experiments suffer from the problem of high-dimensionality. There are a lot more genes than samples available for analysis. So, in this project we decided to identify several microarray datasets that suffer from the curse of dimensionality and apply various feature engineering techniques to reduce the number of genes in each case. Finally, we built classifiers using each of these feature-reduced datasets and compare their accuracies.  
**Category:** Summer internship project at the [Indian Statistical Institute Kolkata](https://www.isical.ac.in/)  
**Funding agency:** [National Network for Mathematical and Computational Biology (NNMCB)](http://www.iiserpune.ac.in/~mbio/?q=nnmcb/internship)  
**Supervisors:** [Dr Subhra Shankar Ray](https://www.isical.ac.in/~shubhra/)  
**Repository:** [Link](https://github.com/banerjeeshayantan/NNMCB-project)  

### 5. Predicting protein functions from interaction data using network features
Predicting function of unknown proteins have been a long standing research problem to determine pathogenicity in target organisms. Computational prediction can be a fast and economical option to achieve that as compared to in-vitro studies. In this report, we try to predict functions of unknown proteins in Saccharomyces cerevisiae using machine learning algorithms and using network properties as features. We achieve reasonable accuracy using Random Forests and a particular type of SVM classifier.  
**Category:** Course project for "Computational Systems Biology"  
**Detailed write-up:** [Link](https://drive.google.com/file/d/1KveTAZzyXxXrK8pudYWT6hkUJR-aBC6I/view?usp=sharing)  





## Electronic health records and machine learning
### 1. Prediction of in-hospital mortality for patients suffering from coronary atherosclerosis using electronic health records
Electronic health records are digitized real-time version of patient records that makes patient information available instantly and securely to authorized users. Coronary artery disease (CAD) often leads to myocardial infraction, which may be fatal. The risk factors associated with this disease are embedded in electronic health records and features can be extracted to build predictive models. After a patient is admitted and the blood tests and clinical data (like Insurance, Admission type and Gender) are collected, predictive models can be built to classify survivability of patients within 30 days of admission. This is the most critical period for surviving coronary atherosclerosis. The main objective of this study was to build five different predictive models using demographic data, treatment data, lab measurements reported within 24 hours of admission, a combined model using all of the above and free text clinical notes. A comparative analysis of the results would then elucidate the best set of features that gives the most predictive power.  
**Category:** Independent research project  
**Repository:** [Link](https://github.com/banerjeeshayantan/CVD_mortality)  
**Detailed write-up:** [Link](https://docs.google.com/document/d/151V6yXZmZnko_lbJX1C0F7RNP7XHd25isx8R8zbZLIE/edit?usp=sharing)  

### 2. SepTrack: An efficient sepsis mortality risk tracker built using machine learning techniques to monitor high-risk patients
Sepsis is a life threatening condition that occurs as a result of the body’s response to infection causing tissue damage and even death. It mostly affects children, the elderly or anyone with a weak immune system. Hospital acquired sepsis is even worse as patients can contract the disease even after the primary ailment is cured. In India the mortality rate of ICU acquired sepsis is very high. Large scale epidemiological studies have shown that clinical parameters can be attributed to high mortality rate among ICU patients. In this project, clinical and demographic data, lab measurements (collected withon 24 hours of admission) and free text clinical notes were used as features to build predictive models to predict 30-day mortality among sepsis patients. This project was chosen as one of the top 15 ideas at the Grand Finale of the Intel Python Hackfury 2019. As a requirement for entering the hackathon, I implemented all the machine learning models using the [Intel DAAL framework](https://software.intel.com/en-us/daal). A comparison of the runtimes between Intel DAAL and sklearn was also completed as part of the analysis.  
**Category:** [Hackathon project](https://plan.seek.intel.com/IntelPythonHackFury-Reg?trackSrc=AIM)  
**Detailed write-up:** [Link](https://docs.google.com/document/d/1eoKGCF26R-LAmJw5b2AvnYH6RfAiiDhnmOx8XAK6X1Y/edit?usp=sharing)  
**Slides:** [Link](https://drive.google.com/file/d/1ecDXFlrhv57mUKc6mPg5GxgbbWHpejx6/view?usp=sharing)  
**Repository:** [Link](https://github.com/banerjeeshayantan/Intel_hackfury_2019)  

### 3. SmartEHR: A web-based tool to analyze free text clinical notes using Natural language processing and Machine learning techniques
A hospital readmission is an episode when a patient who had been discharged from a hospital is admitted again within a specified time interval. Readmission rates have increasingly been used as an outcome measure in health services research and as a quality benchmark for health systems. Hospitals have to face penalities if their readmission rates are high. So, predicting the chances of readmission using the EHR data of patients (like discharge notes) will be of utmost importance. In this project, I used publicly available EHR data to extract free text clinical notes from EHR records and build a web-based interface to predict the 30 day readmission chances, top 5 most probable diagnoses and the top 20 keywords specific to the input document. This tool used popular Natural Language processing and machine learning techniques to preprocess, engineer features and build predcitive models. The web tool was built using the Python Flask framework. This tool was awarded the [first prize](https://rbc-dsai.iitm.ac.in/news/2019/01/11/Shaastra-AI-Challenge.html) in the HSBC AI challenge at Shaastra 2019.  
**Category:** [Hackathon project](https://www.techgig.com/hackathon/SAIC)    
**Slides:** [Link](https://drive.google.com/file/d/1LtLzcDaMawhxbm6NuFGjvZo7U6u45EMM/view?usp=sharing)  
**Repository:** [Link](https://github.com/banerjeeshayantan/SmartEHR)  
**Demo:** [Link](https://rbc-dsai.iitm.ac.in/news/2019/01/11/Shaastra-AI-Challenge.html)  

## Machine learning projects 
### Predicting photometric redshifts using machine learning methods
A photometric redshift is an estimate for the recession velocity of a galaxy without measuring its spectrum. This project was done at [NCRA](ncra.tifr.res.in) under the guidance of [Dr Yogesh Wadadekar](http://www.ncra.tifr.res.in:8081/~yogesh/). The main objective was to accurately predict photometric redshifts and comapre them with methods built on spectroscopic data. A more datailed work on the topic was done by Dr Wadadekar and can be found [here](adsabs.harvard.edu/abs/2005PASP..117...79W). The photometric data from SDSS DR 8-10 was collecetd and popular machine learning methods such as linear regression, support vector regression, artificial neural networks and tree based methods. The rms error in redshift estimation is reported and compared with other existing studies.  
**Category:** Winter internship project  
**Repository:** [Link](https://github.com/banerjeeshayantan/NCRA)  

### Classifying types of particles generated in high energy collider experiments
This project was one of the tasks for the KDD Cup 2004. The goal in this task was to learn a classification rule that differentiates between two types of particles generated in high energy collider experiments. It was a binary classification problem with 78 attributes. The leaderboard ranking was based on four different classification metrics. The [final leaderboard](http://osmot.cs.cornell.edu/cgi-bin/kddcup/newtable.pl?prob=phy) ranking for this task was 87.750.  
**Category:** Assignment for the course "Introduction to Machine learning"  
**Repository:** [Link](https://github.com/banerjeeshayantan/KDD2004)  

### Protein homology prediction task  
The goal for this project was to predict which proteins were homologous to a native sequence. The data was grouped into blocks around each native sequence. 153 native sequences and 150 native sequences were supplied as the training set and the test set respectively. ***The final model gave the best results overall with a second best RMSE of 0.03476 that is within 1% of the RMSE of the winning team.*** The average [leaderboard ranking](http://osmot.cs.cornell.edu/cgi-bin/kddcup/newtable.pl?col=5&order=1&prob=bio) (username: shayantan) across all metrics for this task was 85.5 and for RMSE was 2.   
**Category:** Assignment for the course "Introduction to Machine learning"  
**Repository:** [Link](https://github.com/banerjeeshayantan/KDD2004)  


