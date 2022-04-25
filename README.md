# Mutation-analysis-of-spike-proteins-among-SARS-CoV-2-Variants
| Objectives                                                                                                 |
|------------------------------------------------------------------------------------------------------------|
| Understanding sequence similarity and mutations of different SARS CoV-2 variants                           |
| Illustrating for a specific gene of interest how much the variants are different from the reference genome |

## Introduction

Mutations in the spike region of SARS CoV-2 have been studied to make newer variants wildly contagious and provide advantages to spread faster. So, in this project the gene of interest is spike protein coding gene of SARS CoV-2. 

## Preinstallation 

* Conda to access jupyter https://docs.anaconda.com/anaconda/install/
* Biopython installation. Install it if its not installed yet.  ``` pip install biopython```
* MAFFT Installation in conda ``` conda install -c biocore mafft ```
* matplotlib for the figure ```pip install matplotlib```


## Workflow 

* Sequences for the reference genome (Wuhan strain) of the SARS CoV-2, five variants of concern (B.1.1.7|Alpha, B.1.351|Beta, P.1|Gamma, B.1.617|Delta, B.1.1.529|Omicron) were retrieved from NCBI. 
* Packages Biopython (seqIO) was used to read and manipulate the sequence. 
* Then the sequences was aligned by using MAFFT package.
* Alignment file was produced and went through another arguement to cover the gapped section between the coding regions for spike protein coding genes. 
* Dictionary for the specific gene was created and another test was performed to ensure the alignment process. 
* A variable was assigned to show the mutation on the nucleotide position comparing to the Wuhan strain as that was the reference genome. 
* Using translate function (an inbuilt function in Biopython package), the spike protein coding nucleotides was translated to amino acid sequences.  
* Amino acid sequences are aligned using MAFFT. Mutations type and positions will be turned out through another variable assigned to show the mutations among the amino acid sequences. 
* matplotlib package was used to illustrate the mutations in amino acid sequences from the Wuhan strain of SARS CoV-2.
