---
layout: post
title: March Daily
date: '2023-03-13'
---
Purpose: 
- work log

## 2023-03-13 Monday

### 1. Thought about strategy for candidate gene analysis
Considered whether I should look at (A) difference in mean methylation between genes, or (B) gene-level enrichment in P<0.05 CpGs. 
Eventually decided to go with (B) first since both appear to be the same and I already have
EWAS results

### 2. Read about chi-square testing for enrichment (observed vs expected)
Learnt that chi-square goodness-of-fit and independence tests are mathematically the same. 
Drafted the following plan for my analysis: 

Aim: chi-square goodness-of-fit test to determine: is there deviation from the expected number of 
CpGs found at P<0.05 in a gene if it is associated with disease? 

Steps: 
- identify candidate genes previously associated with DCM 
- calculate number of CpGs tested in a gene
- calculate expected number of CpGs @ P<0.05 in gene 
	- (Expected: 0.05 x no. of CpGs for given threshold of P<0.05) 
- Calculate chi-sq test p-value (which I have not researched yet...)

### 3. Learnt about the different types of variables
Quantitative (numeric)
- continuous
- discrete

Qualitative (categorical)
- ordinal (has levels, e.g. 'low' or 'high' SES) 
- nominal (e.g. race, eye color) 

### 4. Read genetic studies of DCM (ref. 'PhD literature' in Notion) to (A) understand how 'established' 
genes for DCM were determined and to (B) find papers to extract gene lists from. Finalised 3 pass process 
for assessing suitability of papers and tried it out on Dellefave Castillo et al. 


## 2023-03-14 Tuesday

### 1. Read and collated gene lists for candidate gene analysis from 2 DCM genetics papers: 
- largest GWAS by Garnier et al. 2021
- phenotypic refinement by Aragam et al. 2019
Both papers were chosen for sample size; i.e. having largest DCM cohorts

### 2. Git versioning tutorial with Irfan
Notes and useful commands: /Users/konstanzetan/Desktop/PhD/Learning/Git\ /2023-03-14\ Irfan\ versioning.txt 
Learnt about purpose and method of creating branches, sequence of committing edits, meaning 
of pull requests. Add version header to start of new scripts. Branches used for feature development 

### 3. Revise paper selection for candidate gene analysis: using Garnier et al. 2021 and 
Aragam et al. 2019 to prioritise papers. Strategy: "cast nets wide" to include as many 
genomic regions as possible, increasing likelihood of including required CpGs.
