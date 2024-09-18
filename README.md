# Oligonucleotide Library Assisted Sequence Mining Reveals Promoter Sequences With Distinct Temporal Expression Dynamics For Applications In Curvibacter sp. AEP1-3
This repository contains the code for the promotor sequence analysis for *Curvibacter* sp. AEP1-3.
To repeat the analysis steps of the manuscript, download this GitHub-Repository, decompress the file in *data/meta_data.tar.xz* and *data/r2aplus_30degree.tar.xz*.

In addition result files and graphs for all analyzed 5'UTR sequences can be found within the result directory after decompressing *results/r2aplus_30degree_cohorte1.tar.xz* and *results/r2aplus_30degree_cohorte2.tar.xz*. The figures of the original publication and some additional graphs can be obtained by executing the Jupyter Notebook files in a suitable software environment. For this purpose the Docker image at *kanomble/eps_project:1.2* can be used. 

The script *5_prime_utr_curvibacter_sequences.ipynb* was used to search and extract putative promoter regions, as well as to assess those regions for potential binding sites for restriction enzymes.
The script *promotor_project_curvibacter.ipynb* was used to analyse the read counts of the transcriptome analysis and the data obtained from the plate reader measurements.
