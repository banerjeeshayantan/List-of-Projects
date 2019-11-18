# List-of-Projects
## Genomics and machine learning
### Identifying the context of mutations in a cancer genome
Exploring the genomic context of cancer-causing mutations and using that to differentiate between driver and passenger mutations is not very well 
explored. In this study, we use both publicly available cancer mutation data from the [COSMIC v90](https://cancer.sanger.ac.uk/cosmic) and
WGS data from isogenic mice models affected with PDAC to extract sequence-based features from the neighbourhood of a mutation. 
Our goal is to develop novel algorithms that apply methods from Natural Language Processing and machine learning to analyse the sequence and positional 
context of genomic mutations to distinguish between driver and passengers.  

**Supervisors**: [Dr Karthik Raman](https://home.iitm.ac.in/kraman/lab/karthik/) and [Dr Balaraman Ravindran](https://www.cse.iitm.ac.in/~ravi/)  
**Category:** Masters project  
**Report:** A [brief analysis](https://docs.google.com/document/d/13MOsX7WKgRlUIp4-PJP8s5HroQTX2DOOf2WrI2T--vY/edit?usp=sharing) of the results obtained so far.
  
  

### Integrating genomic and clinical data to differentiate between sepsis patients having complicated course outcomes
Sepsis is a life threatning condition and an estimated 4.2 million newborns and children are affected every year. In the first part of this project we analyzed publicly available pediatric sepsis gene expression data [GSE66099](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE66099) to differentiate between survivors and non-survivors. Complicated course outcomes is defined as mortality by 28 days or persistence of greater than or equal to two organ failures at day 7 of septic shock. Using the complicated course labels provided by our [collaborators](https://www.cincinnatichildrens.org/bio/w/hector-wong), we did differential gene expression analysis on the same microarray data. The differentially expressed genes (DEGs) or the biomarkers found in this analysis were validated using already existing studies and functional analysis was also performed. Next, using the same microarray data, we experimented with different feature selection approaches and extracted a set of stable features (genes) for building machine learning models for classifying complicated course vs uncomplicated course patients.  

**Supervisors**: [Dr Rishikesan Kamaleswaran](https://www.kamaleswaran.com/), [Dr Akram Mohammed](https://akram-mohammed.github.io/)  
**Category:** [Google Summer of Code](https://summerofcode.withgoogle.com/organizations/5759105409482752/#5859209076277248) project .   
**Repository:** [Github repo containing proposal, final report and codes](https://github.com/banerjeeshayantan/GSOC-complicated_Course_project).  


