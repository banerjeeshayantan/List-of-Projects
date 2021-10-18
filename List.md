# List-of-Projects

### Table of Contents
=================

   * [List-of-Projects](#list-of-projects)
      * [Genomics and machine learning](#genomics-and-machine-learning)
         * [Project 1: Identifying the context of mutations in a cancer genome](#project-1-identifying-the-context-of-mutations-in-a-cancer-genome)
         * [Project 2: Integrating genomic and clinical data to differentiate between sepsis patients having complicated course outcomes](#project-2-integrating-genomic-and-clinical-data-to-differentiate-between-sepsis-patients-having-complicated-course-outcomes)
         * [Project 3: Integrative analysis and identification of cancer driver genes using publicly available mutation data](#project-3-integrative-analysis-and-identification-of-cancer-driver-genes-using-publicly-available-mutation-data)
         * [Project 4: Classifying cancerous tissue using gene expression data](#project-4-classifying-cancerous-tissue-using-gene-expression-data)
         * [Project 5: Predicting protein functions from interaction data using network features](#project-5-predicting-protein-functions-from-interaction-data-using-network-features)
      * [Electronic health records and machine learning](#electronic-health-records-and-machine-learning)
         * [Project 6: SmartEHR: A web-based tool to analyze free text clinical notes using Natural language processing and Machine learning techniques](#project-6-smartehr-a-web-based-tool-to-analyze-free-text-clinical-notes-using-natural-language-processing-and-machine-learning-techniques)
         * [Project 7: Prediction of in-hospital mortality for patients suffering from coronary atherosclerosis using electronic health records](#project-7-prediction-of-in-hospital-mortality-for-patients-suffering-from-coronary-atherosclerosis-using-electronic-health-records)
         * [Project 8: SepTrack: An efficient sepsis mortality risk tracker built using machine learning techniques to monitor high-risk patients](#project-8-septrack-an-efficient-sepsis-mortality-risk-tracker-built-using-machine-learning-techniques-to-monitor-high-risk-patients)
      * [Machine learning projects](#machine-learning-projects)
         * [Project 9: Predicting photometric redshifts using machine learning methods](#project-9-predicting-photometric-redshifts-using-machine-learning-methods)
         * [Project 10: Classifying types of particles generated in high energy collider experiments](#project-10-classifying-types-of-particles-generated-in-high-energy-collider-experiments)
         * [Project 11: Protein homology prediction task](#project-11-protein-homology-prediction-task)
      * [Others](#others)
         * [Project 12: Understanding Information Privacy Assimilation in IT Organizations using Multi-site Case Studies](#project-12-understanding-information-privacy-assimilation-in-it-organizations-using-multi-site-case-studies)


## Genomics and machine learning
### Project 1: Identifying the context of mutations in a cancer genome
Exploring the genomic context of cancer-causing mutations and using that to differentiate between driver and passenger mutations is a relatively unexplored concept. In this study, we use both publicly available cancer mutation data from the [COSMIC v90](https://cancer.sanger.ac.uk/cosmic) and a [dataset](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006981) of missense mutations from 58 genes with experimentally validated functional and transforming impacts from various studies to extract sequence-based features from the neighbourhoods of mutations. 
Our goal is to develop novel algorithms that apply methods from Natural Language Processing and machine learning to analyse the sequence and positional 
context of genomic mutations to distinguish between driver and passengers. To ensure generalizability, we use five seperate independent validation datasets to test our machine learning tool ****NBDriver****.  

**Supervisors**: [Dr. Karthik Raman](https://home.iitm.ac.in/kraman/lab/karthik/) and [Dr. Balaraman Ravindran](https://www.cse.iitm.ac.in/~ravi/)  
**Category:** Masters project  
**Manuscript:** [Link](https://www.mdpi.com/2072-6694/13/10/2366) to the manuscript recently published in the *Cancers* journal.  
**Poster:** [Link](https://drive.google.com/file/d/1AbDwwrqpjnbNW0-zEiuNSYCAOD4VH9Ho/view?usp=sharing)   
**Conference:** [Presented at the Nextgen Genomics,Biology, Bioinformatics and Technologies Conference 2018 held in Jaipur](https://www.sgrfconferences.org/2018/NGBT/).  
**Tools:** NGS tools like Samtools, Strelka, VEP, GATK etc  
**Languages:** R and Python  
**Duration:** August 2016- May 2021  
**Link to repository:** [NBDriver](https://github.com/RamanLab/NBDriver)  
  

### Project 2: Integrating genomic and clinical data to differentiate between sepsis patients having complicated course outcomes
Sepsis is a life threatning condition and an estimated 4.2 million newborns and children are affected every year. In the first part of this project we analyzed publicly available pediatric sepsis gene expression data [GSE66099](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE66099) to differentiate between survivors and non-survivors. Complicated course outcomes is defined as mortality by 28 days or persistence of greater than or equal to two organ failures at day 7 of septic shock. Using the complicated course labels provided by our [collaborators](https://www.cincinnatichildrens.org/bio/w/hector-wong), we did differential gene expression analysis on the same microarray data. The differentially expressed genes (DEGs) or the biomarkers found in this analysis were validated using already existing studies and functional analysis was also performed. Next, using the same microarray data, we experimented with different feature selection approaches and extracted a set of stable features (genes) for building machine learning models for classifying complicated course vs uncomplicated course patients.  

**Supervisors**: [Dr. Rishikesan Kamaleswaran](https://www.kamaleswaran.com/), [Dr. Akram Mohammed](https://akram-mohammed.github.io/)  
**Category:** [Google Summer of Code](https://summerofcode.withgoogle.com/organizations/5759105409482752/#5859209076277248) project.     
**Slides:** [Link](https://drive.google.com/file/d/12hzYFZTlAtSFICj8AqjTwiGq6gXrfrT_/view?usp=sharing)  
**Initial proposal:** [Proposal](https://drive.google.com/file/d/1h9Q_7oSiNjwGm3zO6ZRPDexxbTu3XdDy/view?usp=sharing)    
**Repository:** [Github repo containing the final report and codes](https://github.com/banerjeeshayantan/GSOC-complicated_Course_project).  
**Tools:** Cytoscape  
**Languages:** R and Python  
**Funding agency:** [Google](https://developers.google.com/open-source/gsoc/help/student-stipends)  
**Duration:** May 2019 - September 2019  
**Manuscript:** [Link to the manuscript recently published in the *Frontiers in Immunology* journal](https://www.frontiersin.org/articles/10.3389/fimmu.2021.592303/)  


### Project 3: Integrative analysis and identification of cancer driver genes using publicly available mutation data
Driver mutations are somatic mutations that help in cancer progression while passenger mutations have no effect on the fitness of a cancer cell. Distinguising drivers from passengers is challenging because drivers occur less frequently than passengers and their functional impact is not intuitively obvious. Several computational approaches have been developed so far to generate a list of high confidence cancer driver genes. In this project, three of the most popular driver prediction tools were used to identify driver genes across six cancer types and their accuracy in terms of overlap with the [Cancer Gene Census](https://cancer.sanger.ac.uk/census) were noted. Mutational load comparison between the downloaded mutation data and TCGA cohorts was performed and a list of common oncogenic pathways affected for each cancer type were validated with the existing literature. Finally, a list of high confidence drivers predicted by all three tools were generated. A short analysis showed that different cancer types share altered genetic components that can be used as prime therapeutic targets.  
  
**Category:** Independent research project based on the findings discussed in the PBS documentary ["Cancer: The Emperor of All Maladies"](https://www.pbs.org/show/story-cancer-emperor-all-maladies/)  
**Detailed write-up:** [Link](http://bit.ly/driver_ind_proj)  
**Repository:** [Link](https://github.com/banerjeeshayantan/Driver_gene_identificantion)  
**Tools:** CanDrA, MutSigCV, OncodriveCLUST  
**Languages:** MATLAB, R, Python  
  
 
 ### Project 4: Classifying cancerous tissue using gene expression data  
DNA microarray technology is used to measure the expression levels of genes under various conditions. Differential expression of these genes can elucidate newer insights into the functioning of various diseases. Usually, microarray experiments suffer from the problem of high-dimensionality. There are a lot more genes than samples available for analysis. So, in this project we decided to identify multiple microarray datasets that suffer from the curse of dimensionality and apply various feature engineering techniques to reduce the number of genes in each case. Finally, we built classifiers using each of these feature-reduced datasets and compared their accuracies.  
  
**Category:** Summer internship project at the [Indian Statistical Institute Kolkata](https://www.isical.ac.in/)  
**Funding agency:** [National Network for Mathematical and Computational Biology (NNMCB)](http://www.iiserpune.ac.in/~mbio/?q=nnmcb/internship)  
**Supervisors:** [Dr Subhra Shankar Ray](https://www.isical.ac.in/~shubhra/)  
**Repository:** [Link](https://github.com/banerjeeshayantan/NNMCB-project)  
**Languages:** R and Python  
**Duration:** June 2015 - August 2015

### Project 5: Predicting protein functions from interaction data using network features
Predicting function of unknown proteins have been a long standing research problem to determine pathogenicity in target organisms. Computational prediction can be a fast and economical option to achieve that as compared to in-vitro studies. In this project, we try to predict functions of unknown proteins in Saccharomyces cerevisiae using machine learning algorithms and network properties as features. We achieve reasonable accuracy using Random Forests and a particular type of SVM classifier.  
  
**Category:** Course project for [Computational Systems Biology](https://home.iitm.ac.in/kraman/lab/courses/2013/bt5240)  
**Detailed write-up:** [Link](https://drive.google.com/file/d/1KveTAZzyXxXrK8pudYWT6hkUJR-aBC6I/view?usp=sharing)  
**Tools:** Cytoscape  
**Languages:** Python  
**Duration:** January 2018 - May 2018





## Electronic health records and machine learning
### Project 6: SmartEHR: A web-based tool to analyze free text clinical notes using Natural language processing and Machine learning techniques
A hospital readmission is an episode when a patient who had been discharged from a hospital is admitted again within a specified time interval. Readmission rates have increasingly been used as an outcome measure in health services research and as a quality benchmark for health systems. Hospitals have to face penalities if their readmission rates are high. So, predicting the chances of readmission using the EHR data of patients (like discharge notes) will be of utmost importance. In this project, I used publicly available EHR data to extract free text clinical notes from EHR records and build a web-based interface to predict the 30 day readmission chances, top 5 most probable diagnoses and the top 20 keywords specific to the input document. This tool used popular Natural Language processing and machine learning techniques to preprocess, engineer features and build predcitive models. The web tool was built using the Python Flask framework. This tool was awarded the [first prize](https://rbcdsai.iitm.ac.in/news/shaastra-ai-challenge/) in the HSBC AI challenge at Shaastra 2019.  
  
**Category:** [Hackathon project](https://www.techgig.com/hackathon/SAIC)    
**Slides:** [Link](https://drive.google.com/file/d/1LtLzcDaMawhxbm6NuFGjvZo7U6u45EMM/view?usp=sharing)  
**Repository:** [Link](https://github.com/banerjeeshayantan/SmartEHR)  
**Demo:** [Link](https://rbc-dsai.iitm.ac.in/news/2019/01/11/Shaastra-AI-Challenge.html)  
**Languages:** SQL, R, Python, Python flask  
**Duration:** November 2018 - January 2019
### Project 7: Prediction of in-hospital mortality for patients suffering from coronary atherosclerosis using electronic health records
Electronic health records are digitized real-time version of patient records that makes patient information available instantly and securely to authorized users. Coronary artery disease (CAD) often leads to myocardial infraction, which may be fatal. The risk factors associated with this disease are embedded in electronic health records and features can be extracted to build predictive models. After a patient is admitted and the blood tests and clinical data (like Insurance, Admission type and Gender) are collected, predictive models can be built to classify survivability of patients within 30 days of admission. This is the most critical period for surviving coronary atherosclerosis. The main objective of this study was to build five different predictive models using demographic data, treatment data, lab measurements reported within 24 hours of admission, a combined model using all of the above and free text clinical notes. A comparative analysis of the results would then elucidate the best set of features that gives the most predictive power.    
  
**Category:** Independent research project  
**Repository:** [Link](https://github.com/banerjeeshayantan/CVD_mortality)  
**Languages:** SQL, R, Python  
**Detailed write-up:** [Link](https://drive.google.com/file/d/1AIHEmGh3YcT9xTbAmkIU2t7tzoMAYVKm/view?usp=sharing)  


### Project 8: SepTrack: An efficient sepsis mortality risk tracker built using machine learning techniques to monitor high-risk patients
Sepsis is a life threatening condition that occurs as a result of the body’s response to infection causing tissue damage and even death. It mostly affects children, the elderly or anyone with a weak immune system. Hospital acquired sepsis is even worse as patients can contract the disease even after the primary ailment is cured. In India the mortality rate of ICU acquired sepsis is very high. Large scale epidemiological studies have shown that clinical parameters can be attributed to high mortality rate among ICU patients. In this project, clinical and demographic data, lab measurements (collected withon 24 hours of admission) and free text clinical notes were used as features to build predictive models to predict 30-day mortality among sepsis patients. This project was chosen as one of the top 15 ideas at the Grand Finale of the Intel Python Hackfury 2019. As a requirement for entering the hackathon, I implemented all the machine learning models using the [Intel DAAL framework](https://software.intel.com/en-us/daal). A comparison of the runtimes between Intel DAAL and sklearn was also completed as part of the analysis.  
  
**Category:** [Hackathon project](https://plan.seek.intel.com/IntelPythonHackFury-Reg?trackSrc=AIM)  
**Detailed write-up:** [Link](https://docs.google.com/document/d/1eoKGCF26R-LAmJw5b2AvnYH6RfAiiDhnmOx8XAK6X1Y/edit?usp=sharing)  
**Slides:** [Link](https://drive.google.com/file/d/1ecDXFlrhv57mUKc6mPg5GxgbbWHpejx6/view?usp=sharing)  
**Repository:** [Link](https://github.com/banerjeeshayantan/Intel_hackfury_2019)  
**Languages:** SQL, R, Python  
**Duration:** August 2019 - September 2019



## Machine learning projects 
### Project 9: Predicting photometric redshifts using machine learning methods
A photometric redshift is an estimate for the recession velocity of a galaxy without measuring its spectrum. This project was done at the [NCRA](http://www.ncra.tifr.res.in/ncra/main) under the guidance of [Dr Yogesh Wadadekar](http://www.ncra.tifr.res.in:8081/~yogesh/). The main objective was to accurately predict photometric redshifts and compare them with methods built on spectroscopic data. A more detailed work on the topic was done by Dr Wadadekar and can be found [here](https://ui.adsabs.harvard.edu/abs/2005PASP..117...79W/abstract). The photometric data from SDSS DR 8-10 was collected and popular machine learning methods such as linear regression, support vector regression, artificial neural networks and tree based methods. The rms error in redshift estimation is reported and compared with other existing studies.  
  
**Category:** Winter internship project  
**Funding agency:** [National Centre for Radio Astrophysics](http://www.ncra.tifr.res.in/ncra/main)  
**Repository:** [Link](https://github.com/banerjeeshayantan/NCRA)  
**Languages:** R  
**Duration:** January 2015 - February 2015

### Project 10: Classifying types of particles generated in high energy collider experiments
This project was one of the tasks for the KDD Cup 2004. The goal in this task was to learn a classification rule that differentiates between two types of particles generated in high energy collider experiments. It was a binary classification problem with 78 attributes. The leaderboard ranking was based on four different classification metrics. The [final leaderboard](http://osmot.cs.cornell.edu/cgi-bin/kddcup/newtable.pl?prob=phy) ranking for this task was 87.750.  
  
**Category:** Assignment for the course "Introduction to Machine learning"  
**Repository:** [Link](https://github.com/banerjeeshayantan/KDD2004)  
**Languages:** Python  
**Duration:** January 2019 - May 2019

### Project 11: Protein homology prediction task  
The goal for this project was to predict which proteins were homologous to a native sequence. The data was grouped into blocks around each native sequence. The training set had 153 native sequences and the testing set had 150 native sequences. ***The final model gave the best results overall with a second best RMSE of 0.03476 that was within 1% of the RMSE of the winning team.*** The average [leaderboard ranking](http://osmot.cs.cornell.edu/cgi-bin/kddcup/newtable.pl?col=5&order=1&prob=bio) (username: shayantan) across all metrics for this task was 85.5 and for RMSE was 2.   
  
**Category:** Assignment for the course "Introduction to Machine learning"  
**Repository:** [Link](https://github.com/banerjeeshayantan/KDD2004)  
**Languages:** R and Python  
**Duration:** January 2019 - May 2019
## Others
### Project 12: Understanding Information Privacy Assimilation in IT Organizations using Multi-site Case Studies
Immerse, the institute research magazine, is the annual science publication of The Fifth Estate. It stands for IIT Madras Magazine on Research in Science and Engineering, where the endeavour is not only to showcase some of the recent developments in research and innovation at IIT Madras, but also to communicate the science behind them in the simplest way possible for better understanding and appreciation. The student writers are usually encouraged to choose their favourite research lab within the institute (preferably outside their own department or area of expertise). Then after multiple interviews with the PI and the researchers of that lab along with multiple rounds of editing, the final article is produced. Last year, I was very fortunate to interview [Dr Saji Mathew](https://doms.iitm.ac.in/index.php/skm) from the Department of Management Studies in IIT Madras. His area of interest revolves around Web personalization and Information privacy.   
  
**Category:** Magazine article  
**Article:** [Link](https://drive.google.com/file/d/12PLOmF0nrPvLqCB8uLicvWRL0ieEMLnk/view?usp=sharing) (Turn to Page 10 for the article).  
**Duration:** October 2018 - December 2018


