NOTES: 
- Really incomplete
- Pipeline for getting fasta files to vcf files
- fasta files are mapped to reference using minimap2, whose mappings end up as paf files
- paf files are parsed to vcfs with a script
- vcfs are normed and then merged with bcftools norm and bcftools merge respectively
- Pipeline is wrapped with snakemake
- IMPORTANT: make sure to install conda env whose .yml is found in "env" directory


- paftools.js is from the minimap2 package by lh3
- Pipeline makes use of Snakemake and conda environments
- samples dir is to be filled with .fna (fasta) files of whole genome assemblies
- ref dir should contain reference genome assembly and associated index file (.fai)
- conda environment from envs should be created by user and activated before calling snakemake
