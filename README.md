# Python-For-Variant-Calling
Variant calling is an essential downstream analysis in Next Generation Sequencing analysis. Filtering variants in sequenced DNA samples is an essential process towards determining variations in the samples
relative to the reference sequence. While typically written in bash script, the pipeline script in this repo is coded in Python (filename: variant-caller.py), which is the chosen programming language for this pipeline because of its powerful functionalities that enable developers to track bugs, unit-test codes, build control and automation.
The pipeline employs an inital software-like user friendly interface which checks that the right file naming convention compatible with the pipeline is used by user.

The pipeline uses the following python modules for its processing: os, glob, os.path and subprocess ( importing call).

From input fastq files, the pipeline generates VCF files, and also filters the files to seperately generate indels and snv VCFs. 
VCF file filtering is an essential step added for researh purpose. For instance, concatenation of indels and snvs variants from tumour samples may be used as inputs in the pipeline for generating mutation table used in somatic cancer driver analysis that employs Non Synonymous:Synonymous mutation ratio (Martincorena, et al., 2017)

Reference

Martincorena I, Raine KM, Gerstung M, Dawson KJ, Haase K, Van Loo P, Davies H, Stratton MR, Campbell PJ. Universal Patterns of Selection in Cancer and Somatic Tissues. Cell. 2017 Nov 16;171(5):1029-1041.e21. doi: 10.1016/j.cell.2017.09.042. Epub 2017 Oct 19. Erratum in: Cell. 2018 Jun 14;173(7):1823. PMID: 29056346; PMCID: PMC5720395.
