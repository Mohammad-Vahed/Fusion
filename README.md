# Fusion

## An innovative bioinformatics pipeline for detecting and characterizing fusion transcripts in breast cancer and healthy cell lines


# Fusion Transcript Detection Pipeline
This repository contains an advanced bioinformatics pipeline designed for the identification and characterization of fusion transcripts in breast cancer and normal cell lines. The pipeline leverages cutting-edge algorithms to analyze RNA sequencing data, providing insights into the role of gene fusions in cancer biology.

# Key Features
Accurate Detection: Identifies fusion transcripts with high precision and recall.
Comprehensive Analysis: Characterizes the biological relevance of detected fusions in both cancerous and normal cell lines.
User-Friendly Workflow: Easy-to-follow scripts and modular code structure for seamless data processing.

Requirements:
Python (>=3.7)
R (>=4.0)
Necessary bioinformatics tools: [list specific tools, e.g., STAR, FusionCatcher]


Simple run

Run docker image:

bsub -Is -q 'dinglab-interactive general-interactive' -G compute-dinglab -M 100G -R 'select[mem>100G] span[hosts=1] rusage[mem=100G]' -a 'docker(mvahed/fusion)' /bin/bash -l

Run bash:
bash fusion_pipeline_ris_v1_5.sh <Folder of bam files> <File_R1.bam> <File_R2.bam> <CPU "20">
