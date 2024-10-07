# Oligonucleotide Library Assisted Sequence Mining Reveals Promoter Sequences With Distinct Temporal Expression Dynamics For Applications In Curvibacter sp. AEP1-3
This repository contains the code for the promotor sequence analysis for *Curvibacter* sp. AEP1-3.
To repeat the analysis steps of the manuscript, download this GitHub-Repository, decompress the file in *data/meta_data.tar.xz* and *data/r2aplus_30degree.tar.xz*.

In addition result files and graphs for all analyzed 5'UTR sequences can be found within the result directory after decompressing *results/result_set_1.tar.gz* and *results/result_set_2.tar.gz*. The figures of the original publication and some additional graphs can be obtained by executing the Jupyter Notebook files in a suitable software environment. For this purpose the Docker image at *kanomble/curvibacter_promoter_studies:1.0* can be used.
After downloading and decompresssing the GitHub repository, open a terminal and ```cd``` into this directory. Once your terminal points to this directory, run a container with following docker command:

```docker run -dt --name curvibacter_promoter_studies -v ${PWD}:/BigData/applications -p 127.0.0.1:8888:8888/tcp kanomble/curvibacter_promoter_studies:1.0```

This command will automatically pull the required docker image, create and run the container with a Jupyter Notebook server.
The script *5_prime_utr_curvibacter_sequences.ipynb* was used to search and extract putative promoter regions, as well as to assess those regions for potential binding sites for restriction enzymes.
The script *promotor_project_curvibacter.ipynb* was used to analyse the read counts of the transcriptome analysis and the data obtained from the plate reader measurements.
