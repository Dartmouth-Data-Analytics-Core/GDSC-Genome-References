# GDSC Genome References
Instructions for locating and using genome references hosted by the Data Analytics Core on DartFS/Discovery.

<img src="https://github.com/Dartmouth-Data-Analytics-Core/DAC-RNAseq-pipeline/blob/master/img/cqb_logo.jpg" alt="CQB Logo" width="200" align="right"/>

## Root location
Genome references for commonly used organisms and bioinformatics tools can be found at:
```
/dartfs/rc/nosnapshots/G/GMBSR_refs
```

## Genomes and versions available (Last updated 9/23/26)
| Organism | Assembly | Annotation | Indices available |
|---|---|---|---|
| *Homo sapiens* | GRCh38 (GENCODE primary assembly) | GENCODE v45 | BWA, Bowtie2, HISAT2, STAR, RSEM, Picard |
| *Mus musculus* | GRCm39 (GENCODE primary assembly) | GENCODE vM34 | BWA, Bowtie2, HISAT2, STAR, RSEM, Picard |
| *Mus musculus* | mm10 (small RNA annotation only) | Ensembl + miRBase + GtRNAdb | GTF only |
| *Danio rerio* | danRer11 | Lawson Lab V4.3.2 | BWA, Bowtie2, HISAT2, STAR, RSEM, Picard |
| *Drosophila melanogaster* | BDGP6.54 (FlyBase r6.63, FB2025_02) | Ensembl 114 | STAR, Picard |
| *Caenorhabditis elegans* | WBcel235 (WormBase ParaSite WBPS19) | WBPS19 canonical geneset | FASTA + GTF only |

> **STAR version note:** All `STAR_index` directories were built with **STAR 2.7.10a** (updated 4/25/24). Indices built with STAR 2.7.1a are kept in `STAR_2.7.1a_index` for older pipelines.


## Absolute paths to references and indices
#### Homo sapiens GRCh38
```
# Genome fasta file (+ .fai)
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/downloads/GRCh38.primary_assembly.genome.fa
# Gencode v45 annotation GTF file
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/downloads/gencode.v45.annotation.gtf

# BWA genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/dna_index/BWA_index/GRCh38.primary_assembly.genome
# Bowtie2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/dna_index/bowtie2_index/GRCh38.primary_assembly.genome

# Hisat2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/rna_index/hisat2_index/GRCh38.primary_assembly.genome
# STAR genome index (STAR 2.7.10a)
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/rna_index/STAR_index/GRCh38.primary_assembly.genome
# STAR genome index (legacy, STAR 2.7.1a)
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/rna_index/STAR_2.7.1a_index/GRCh38.primary_assembly.genome
# RSEM transcriptome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/rna_index/RSEM_index/GRCh38.primary_assembly.genome

# Picard rRNA interval list and refFlat files
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/annotation/picard/GRCh38.primary_assembly.genome.refFlat
/dartfs/rc/nosnapshots/G/GMBSR_refs/Hsapiens/GRCh38/annotation/picard/GRCh38.primary_assembly.genome.rRNA.interval.list
```

#### Mus musculus GRCm39
```
# Genome fasta file (+ .fai)
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/downloads/GRCm39.primary_assembly.genome.fa
# Gencode vM34 annotation GTF file (a sorted + indexed copy is also available)
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/downloads/gencode.vM34.annotation.gtf
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/downloads/gencode.vM34.annotation.sorted.gtf

# BWA genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/dna_index/BWA_index/GRCm39.primary_assembly.genome
# Bowtie2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/dna_index/bowtie2_index/GRCm39.primary_assembly.genome

# Hisat2 genome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/rna_index/hisat2_index/GRCm39.primary_assembly.genome
# STAR genome index (STAR 2.7.10a)
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/rna_index/STAR_index/GRCm39.primary_assembly.genome
# STAR genome index (legacy, STAR 2.7.1a)
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/rna_index/STAR_2.7.1a_index/GRCm39.primary_assembly.genome
# RSEM transcriptome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/rna_index/RSEM_index/GRCm39.primary_assembly.genome

# Picard rRNA interval list and refFlat files
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/annotation/picard/GRCm39.primary_assembly.genome.refFlat
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/GRCm39/annotation/picard/GRCm39.primary_assembly.genome.rRNA.interval.list
```

#### Mus musculus mm10 (small RNA annotation)
```
# mm10 GTF (chr-prefixed) combining Ensembl genes, miRBase miRNAs and GtRNAdb tRNAs, for small RNA-seq
/dartfs/rc/nosnapshots/G/GMBSR_refs/Mmusculus/mm10_smRNA/genes.gtf.gz
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
# STAR genome index (STAR 2.7.10a)
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/rna_index/STAR_index/danRer11.primary
# STAR genome index (legacy, STAR 2.7.1a)
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/rna_index/STAR_2.7.1a_index/danRer11.primary
# RSEM transcriptome index
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/rna_index/RSEM_index/danRer11.primary

# Picard rRNA interval list and refFlat files
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/annotation/picard/danRer11.primary.refFlat
/dartfs/rc/nosnapshots/G/GMBSR_refs/Drerio/danRer11/annotation/picard/danRer11.primary.rRNA.interval.list
```

#### Drosophila melanogaster BDGP6.54 (FlyBase r6.63 / FB2025_02)
```
# Genome fasta file
/dartfs/rc/nosnapshots/G/GMBSR_refs/drosophila/flybase_dmel_r6.63_FB2025_02/fasta/Drosophila_melanogaster.BDGP6.54.dna.toplevel.fa
# Ensembl 114 annotation GTF file
/dartfs/rc/nosnapshots/G/GMBSR_refs/drosophila/flybase_dmel_r6.63_FB2025_02/annotation/Drosophila_melanogaster.BDGP6.54.114.gtf

# STAR genome index (STAR 2.7.10a)
/dartfs/rc/nosnapshots/G/GMBSR_refs/drosophila/flybase_dmel_r6.63_FB2025_02/rna_index/Drosophila_melanogaster.BDGP6.54.dna.toplevel

# Picard rRNA interval list and refFlat files
/dartfs/rc/nosnapshots/G/GMBSR_refs/drosophila/flybase_dmel_r6.63_FB2025_02/annotation/Drosophila_melanogaster.BDGP6.54.dna.toplevel.refFlat
/dartfs/rc/nosnapshots/G/GMBSR_refs/drosophila/flybase_dmel_r6.63_FB2025_02/annotation/Drosophila_melanogaster.BDGP6.54.dna.toplevel.rRNA.interval.list
```

#### Caenorhabditis elegans WBcel235 (WormBase ParaSite WBPS19)
```
# Genome fasta file (+ .fai; gzipped copy also available)
/dartfs/rc/nosnapshots/G/GMBSR_refs/C_elegans/caenorhabditis_elegans.PRJNA13758.WBPS19.genomic.fa
# WBPS19 canonical geneset GTF file (gzipped copy also available)
/dartfs/rc/nosnapshots/G/GMBSR_refs/C_elegans/caenorhabditis_elegans.PRJNA13758.WBPS19.canonical_geneset.gtf

# No aligner indices built yet. See C_elegans/README.txt for source details.
```

## Other reference databases
```
# BLAST nucleotide databases (NCBI nt, split into eukaryotic and prokaryotic subsets; taxdb included)
/dartfs/rc/nosnapshots/G/GMBSR_refs/blast_DBs/nt_euk/nt_euk
/dartfs/rc/nosnapshots/G/GMBSR_refs/blast_DBs/nt_prok/nt_prok

# Centrifuger index: RefSeq archaea/bacteria/viral + human (build commands in mgx_db/code.txt)
/dartfs/rc/nosnapshots/G/GMBSR_refs/mgx_db/refseq_abvh
# Centrifuger index: GTDB r226 + RefSeq
/dartfs/rc/nosnapshots/G/GMBSR_refs/mgx_db/gtdb_r226+refseq_hvfc/cfr_gtdb_r226+refseq_hvfc

# MetaPhlAn database (mpa_vOct22_CHOCOPhlAnSGB_202212)
/dartfs/rc/nosnapshots/G/GMBSR_refs/mgx_pipeline/metaphlan/metaphlan_databases
# HUMAnN databases: ChocoPhlAn v201901_v31, UniRef90 (full + EC-filtered), UniRef50 (EC-filtered), utility mapping
/dartfs/rc/nosnapshots/G/GMBSR_refs/mgx_pipeline/Choco/chocophlan
/dartfs/rc/nosnapshots/G/GMBSR_refs/mgx_pipeline/uniref
/dartfs/rc/nosnapshots/G/GMBSR_refs/mgx_pipeline/utility_mapping
```

## Instructions for use with DAC RNA-Seq pipeline
Pre-built configuration files and instructions for using the DAC RNA-Seq pipeline with these references are available in the [RNA-Seq pipeline repository](https://github.com/Dartmouth-Data-Analytics-Core/DAC-RNAseq-pipeline/blob/master/README.md#running-the-pipeline-using-pre-built-references-and-config-files-on-discovery).

**Contact & questions:**
Please address questions to *DataAnalyticsCore@groups.dartmouth.edu* or submit an issue in the GitHub repository.
