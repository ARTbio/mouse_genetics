### Notes on docker image mousegenetics_17.05

- issue with 17.09 for vcfgzfile datatype --> roll back to release_17.05
- run_datamanager does not works beyond the first step (key) in docker
- adapt delegated upload
- load manually bam_coverage tool (deeptools)
- make /tmp/slurm 777 - or do not export /tmp when launching the container
- add in galaxy.ini:
```
display_servers = hgw1.cse.ucsc.edu,hgw2.cse.ucsc.edu,hgw3.cse.ucsc.edu,hgw4.cse.ucsc.edu,hgw5.cse.ucsc.edu,hgw6.cse.ucsc.edu,hgw7.cse.ucsc.edu,hgw8.cse.ucsc.edu,lowepub.cse.ucsc.edu,genome.ucsc.edu
```
