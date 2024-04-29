# DAC-Genome-References 
Instructions for locating and using genome references hosted by the Data Analytics Core on DartFS/Discovery.  

## Root location 
Genome references for commonly used organisms and bioinformatics tools can be found at: 
```
/dartfs/rc/nosnapshots/G/GMBSR_refs
```

## Genomes and versions available (Last updated 3/11/24 )
 - Homo sapiens
   - GRCh38
 - Mus musculus
   - GRCm39 
 - Danio rerio 
   - danRer11
  

## Absolute paths to references and indices
#### Homo sapiens GRCh38
```
# Genome fasta file
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/downloads/GRCh38.primary_assembly.genome.fa
# Gencode v45 annotation GTF file
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/downloads/gencode.v45.annotation.gtf

# BWA genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/dna_index/BWA_index/GRCh38.primary_assembly.genome
# Bowtie2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/dna_index/bowtie2_index/GRCh38.primary_assembly.genome

# Hisat2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/rna_index/hisat2_index/GRCh38.primary_assembly.genome
# STAR genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/rna_index/STAR_index/GRCh38.primary_assembly.genome
# RSEM transcriptome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/rna_index/RSEM_index/GRCh38.primary_assembly.genome

# Picard interval rRNA interval list and refFlat files
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/annotation/picard/GRCh38.primary_assembly.genome.refFlat
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/annotation/picard/GRCh38.primary_assembly.genome.rRNA.interval.list
```

#### Mus musculus GRCh39
```
# Genome fasta file
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/downloads/GRCm39.primary_assembly.genome.fa
# Gencode vM34 annotation GTF file
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/downloads/gencode.vM34.annotation.gtf

# BWA genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/dna_index/BWA_index/GRCm39.primary_assembly.genome
# Bowtie2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/dna_index/bowtie2_index/GRCm39.primary_assembly.genome

# Hisat2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/rna_index/hisat2_index/GRCm39.primary_assembly.genome
# STAR genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/rna_index/STAR_index/GRCm39.primary_assembly.genome
# RSEM transcriptome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/rna_index/RSEM_index/GRCm39.primary_assembly.genome

# Picard interval rRNA interval list and refFlat files
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/annotation/picard/GRCm39.primary_assembly.genome.refFlat
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/annotation/picard/GRCm39.primary_assembly.genome.rRNA.interval.list
```

#### Danio rerio danRer11
```
# Genome fasta file
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/downloads/danRer11.primary.fa
# V4.3.2 validated annotation GTF file
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/downloads/V4.3.2.validated.gtf

# BWA genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/dna_index/BWA_index/danRer11.primary
# Bowtie2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/dna_index/bowtie2_index/danRer11.primary

# Hisat2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/rna_index/hisat2_index/danRer11.primary
# STAR genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/rna_index/STAR_index/danRer11.primary
# RSEM transcriptome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/rna_index/RSEM_index/danRer11.primary

# Picard interval rRNA interval list and refFlat files
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/annotation/picard/danRer11.primary.refFlat
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/annotation/picard/danRer11.primary.rRNA.interval.list
```

## Instructions for use with DAC RNA-Seq pipeline
Pre-built configuration files and instructions for the DAC RNA-Seq pipeline in conjunction with these references are available in the [RNA-Seq pipeline repository]([https://github.com/Dartmouth-Data-Analytics-Core/DAC-Genome-References](https://github.com/Dartmouth-Data-Analytics-Core/DAC-RNAseq-pipeline/blob/master/README.md#running-the-pipeline-using-pre-built-references-and-config-files-on-discovery)).  


**Contact & questions:** 
Please address questions to *DataAnalyticsCore@groups.dartmouth.edu* or submit an issue in the GitHub repository. 
