# VET (Variant Enrichment Testing)

This code can be used to test whether a set of foreground variants is over-represented in a set of genomic locations compared to a set of background variants. 

The foreground set could be, for instance, a set of variants found to affect a molecular phenotype (in QTL-type study). The genomic locations could be, for instance, disease-associated LD-blocks at genome-wide significant GWAS tag SNPs. This could could then be used to answer the following question

*Is the foreground set of variants significantly over-represented in the set of genomic locations compared to the background set?*

The code is based on the concept of bootstrapping simulations. Let F = {1, ..., m} be the foreground set,  B = {1, ..., n} with n >> m and G the set of genomic locations.   If we select N (where N is a very large number, say 1,000 or 10,000) sets of m variants each from B, we can compare the number of intersection of (F,G) and of {(B_1,G), ..., (B_N,G)}

TODO
