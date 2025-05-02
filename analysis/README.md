### README for analysis/ ###

This directory contains X pairs of .Rmd and .html files, plus a subdirectory of fastQC reports:
07_Composition
06_Ordination
05_Biodiversity
04B_Phylogenetic_Tree_Inspection
04A_Phylogenetic_Tree_Construction
03_PreProcessing
02_Assigning_ASV
 01_QualityTrimming

## 07_Composition:
Perform compositional analysis of the scaled/noramlized/rarefied snail intestinal-microbiome dataset. Investigate relative-abundance shifts in taxa within 3 phyla: Pseudomonadota, Bacillota, and Bacteroidetes

## 06_Ordination:
Calculate community dissimilarities between the 6 experimental groups (high, control, low temperatures vs female and male hosts) with: Sorensen, Bray-Curtis, and weighted/unweighted UNIFRAC. Visualize the community data with PCoA and NMDS

## 05_Biodiversity:
Plot and analyze richness, shannon, simpson Hill alpha diversity metrics for 6 experimental groups (high, control, low temperatures vs female and male hosts)

## 04B_Phylogenetic_Tree_Inspection:
Inspect, prune, and midpoint-root the phylogenetic tree created in `04A_Phylogenetic_Tree_Construction`

## 04A_Phylogenetic_Tree_Construction:
Make a phylogenetic tree of the ASVs in our snail microbiome samples in order to conduct phylogenetic community analyses like phylogenetic Hill Numbers and the UniFrac beta-diversity measures

## 03_PreProcessing:
Combine `asv_table`, `tax_table`, and metadata and create phyloseq object. Then, remove any potential contaminants and evaluate the accuracy of the sequencing run, to consolidate into a `raw_preprocessed_physeq` phyloseq data object. 

## 02_Assigning_ASV
Merge, assign ASVs and taxonomy, and and quality-trim filtered fastqs, in order to further process and analyze the 16S sequencing reads

## 01_QualityTrimming
Assess the quality of reads, filter and trim low-quality sequences, and merge reads in order to assign ASV’s downstream
