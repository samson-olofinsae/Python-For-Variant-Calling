# Python-For-Variant-Calling
Variant calling is an essential downstream analysis in Next Generation Sequencing analysis. Filtering variants in sequenced DNA samples is an essential process towards determining variations in the samples
relative to the reference sequence. While typically written in bash script, the pipeline script in this repo is coded in Python, which is the chosen programming language for this 
pipeline because of its powerful functionalities that enable developers to track bugs, unit-test codes, build control and automation.

The pipeline uses the following python modules for its processing: os, glob, os.path and subprocess ( importing call).

From input fastq files, the pipeline generates VCF files, and also filters the files to generate indels and snv VCFs. 
VCF file filtering is an essential step added for researh purpose. For instance, concatenation of indels and snvs variants from tumour samples may be used as inputs for generating mutation tables used in cancer driver analysis such as Non Synonymous:Synonymous mutation ratio
