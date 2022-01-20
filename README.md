# Fusion

Simple run
Run docker image:
bsub -Is -q 'dinglab-interactive general-interactive' -G compute-dinglab -M 100G -R 'select[mem>100G] span[hosts=1] rusage[mem=100G]' -a 'docker(mvahed/fusion)' /bin/bash -l

Run bash:
bash fusion_pipeline_ris_v1_5.sh <Folder of bam files> <File_R1.bam> <File_R2.bam> <CPU "20">
