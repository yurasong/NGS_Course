# NGS Course, Session 1: Introduction to Galaxy and NGS Data Structures

# Updates

 - Please post the errors or questions on the **issue** tab on Github. This will make a record regarding solution and errors.
 - Still you could send us an email.

# Aim of course
 - We will use **Galaxy**
 - Allow you to go from raw data to analysis
 - Teach the steps and associated tools for analysis pipeline
 - Independent to work with NGS datasets
 - Develop Galaxy workflows for new analysis and pipeline : **automation**
 - Analysis of bulk RNA-seq and bulk ATAC-seq from Illumina platform

# File type and procession in NGS dataset

## Raw data

 1. fastq format : fastq format with quality scores
  - Composed of header and sequence
  - Few giga-bytes of files

 2. Trimming of fastq based on the quality
  - To trim out the regions which have low quality
  - K-mers : lack of complexity after trimming due to the lack of adapter info
  - Average of length will be changed and some could be shorter than sequenced length

## Mapping to the genome
 - Using HISAT2 : put trimmed fastq files
 - Reference genome : **Have to use UCSC, built-in genome** because galaxy is connected to UCSC. **The genome and transcriptome information from UCSC and Ensembl are totally different**!!
