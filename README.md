# aCGHarrayDirectHG19
Shell script which allowed to remove european CNV polymorphism and annotate downstream genomic intervals on HG19 human genome especially with cancer genes from COSMIC database, pluripotent genes from Plurinet database, and transcription factor molecules.

This script needs the installation of Bedtools utilities in the OS environement.
This script also needs dependencies of installing 5 annotation databases in the subfolder DATABASES_HG19:

- hg19GENEname_sorted.bed: Refseq HG19 annotations
- scandbHG19CEU_sorted.bed: CNV polymorphisms in european population, data derived from http://www.scandb.org/ website
- plurinetHG19_sorted.bed: genes that are characterized as belonging to a pluripotency network (PLURINET DB)
- CosmicHG19.bed: genes presenting somatic alteration in cancer and leukemia
- TFHG19: census database of molecules classed as transcription factor

Script needs to be execute in BASH environnement with previous dependencies:

USAGE:
$sh acgh_direct_HG19.sh example.bed 

EXAMPLE FILE:
"example.bed" with minimum 5 columns needs to be pass as first parameter of the shell line of execution 
