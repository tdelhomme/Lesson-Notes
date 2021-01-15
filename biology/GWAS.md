# Genome Wide Association Studies

## GWAS artefacts and eQTL

#### Population stratification
If some SNPs are unique to a particular ethnic group, then using multiple ethnicities would dilute the signal and potentially create artifacts.  
If one makes a qq-plot for SNPs in merged populations (one p-value per SNP), it can be that the p-values present an inflation and do not follow the expectations -- this is due to population stratification which is not identical in both case and control groups (because two different populations have different disease frequencies): the significance of p-values is due to different allele frequencies in the populations and not due to different allele frequencies in the cases versus controls.  
* it is crucial to differentiate between variable ethnicity groups

#### Relative samples
In a particular dataset, it can be that 2 samples are relative (from the same family in a sense) but they do not know (and so we do not know). It is also crucial to detect those because they can also skew the statistic.
To measure the relatedness between 2 individuals: IBD (Identity By Descent)

#### Location of significant GWAS SNPs
Majority of GWAS SNPs are located in non-coding regions of the genome :89% of 465 estimated GWAS SNPs were found to be in non-coding according to Hindorff *et al.* PNAS 2009 using the available GWAS catalog. Note that the coding region of the genome is around 1% and we have 11% of GWAS SNPs in genes so we have an 11-fold enrichment compared to what is expected by randomness. In addition, 80% of these 11% are non-synonymous SNPs.

#### eQTL
Then what can we do to link them to genes?
* expression Quantitative Trait Loci analysis: one can estimate the association between a particular SNP allele and the expression of a particular gene, *i.e.* does having this allele increase/reduce the expression of the gene?
* people tend to use GTEx data (Genotype-Tissue expression)
  * 1K individuals
  * 54 non-disease related tissues

#### Epigenetic data for GWAS interpretation
Majority of traits are polygenic (affected by multiple variants). Then one can not simply take the few significant SNPs (because not a few) and look at their positions in the genes or in the non-coding regions (keeping in mind that majority of GWAS SNPs were found in non-coding parts of the genome).

![](figures/kellis2014.jpg)
