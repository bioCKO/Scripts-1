# Scripts
#Make sure that these tools are installed in your system and specify the paths to each tool.

1.Build index

perl BWA_genome_index.pl /your/path/to/genome/prefix.fa

2.Run RNA_editing_identify.sh

sh RNA_editing_identify.sh /your/path/to/genome/prefix SRR_number 

3.Filtering RNA editing sites

sh Filter.sh SRR_number SNP.vcf Splicing.region.bed

Note:
(1).SRR_number should be the sra number or the basename of clean.fq.gz files. For example, SRR123456_1.clean.fq.gz, SRR123456_2.clean.fq.gz. The sequencing fastq files should be located in current directory.
(2).SNP.vcf should be the genome SNPs annotated VCF file. 
(3).Splicing.region.bed should be the genome splicing regions, which could be generated by STAR and HISAT2.
