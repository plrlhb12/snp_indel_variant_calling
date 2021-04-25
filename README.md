# snp_indel_variant_calling

These are jupyter notebooks for doing varaint calling on snp/indel for the Illumina whole genome sequencing data using GATK4 best practices pipeline.
The executation was done on google cloud.

- The germline single nucleotide polymorphism (SNP) and insertion/deletion (indel) variants were called using the HaplotypeCaller (link) following the Genome Analysis Toolkit (GATK) best practices and executed through the Google genomics alpha pipeline. 
- FASTQ files were processed into unmapped BAM files using the paired-fastq-to-unmapped-bam workflow on the human GRCh38 build. The initial variant calling, i.e., the generation of GCVF files, was performed using the PairedSingleSampleWf. 
- The joint discovery was then executed using the JointGenotypingWf. 
- Variants were filtered using the variant quality score recalibration (VQSR) with default filtering parameters. 
