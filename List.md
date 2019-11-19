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
  
  

### 2. Integrating genomic and clinical data to differentiate between sepsis patients having complicated course outcomes
Sepsis is a life threatning condition and an estimated 4.2 million newborns and children are affected every year. In the first part of this project we analyzed publicly available pediatric sepsis gene expression data [GSE66099](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE66099) to differentiate between survivors and non-survivors. Complicated course outcomes is defined as mortality by 28 days or persistence of greater than or equal to two organ failures at day 7 of septic shock. Using the complicated course labels provided by our [collaborators](https://www.cincinnatichildrens.org/bio/w/hector-wong), we did differential gene expression analysis on the same microarray data. The differentially expressed genes (DEGs) or the biomarkers found in this analysis were validated using already existing studies and functional analysis was also performed. Next, using the same microarray data, we experimented with different feature selection approaches and extracted a set of stable features (genes) for building machine learning models for classifying complicated course vs uncomplicated course patients.  

**Supervisors**: [Dr Rishikesan Kamaleswaran](https://www.kamaleswaran.com/), [Dr Akram Mohammed](https://akram-mohammed.github.io/)  
**Category:** [Google Summer of Code](https://summerofcode.withgoogle.com/organizations/5759105409482752/#5859209076277248) project .   
**Initial proposal:** [Proposal](https://github.com/banerjeeshayantan/GSOC-complicated_Course_project/blob/master/GSOC-proposal.pdf)  
**Funding agency:** [Google](https://developers.google.com/open-source/gsoc/help/student-stipends)
**Repository:** [Github repo containing the final report and codes](https://github.com/banerjeeshayantan/GSOC-complicated_Course_project).  


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



