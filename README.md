# Mus musculus RNA-seq Analysis

**Project title:**  
Differential gene expression in mammary gland – Virgin mouse vs 18.5 days pregnancy

**What I did (all in Galaxy + Excel + KOBAS):**

1. Downloaded 4 RNA-seq SRA files from Zenodo  
2. Converted to FASTQ  
3. Quality check: FastQC (before and after trimming)  
4. Trimmed adapters and low quality: Trim Galore  
5. Aligned to mm10 mouse genome: Bowtie2  
6. Count reads per gene: featureCounts → gene count matrix  
7. Differential expression: DESeq2 → found up/down regulated genes  
8. Generated heatmap of expression patterns  
9. Downloaded DESeq2 results → opened in Excel → filtered genes with padj < 0.05  
10. Used significant gene IDs in KOBAS → found enriched pathways  
11. Variant calling (optional): DeepVariant + HeatMap2 visualization

**Files in this repository:**

- `screenshots/` → pictures from every major step in Galaxy  
- `results/` → gene count matrix, DESeq2 table, filtered significant genes, KOBAS pathways

**Original dataset:**  
https://zenodo.org/records/4249555

**Done by:** Suchirayu Karmakar  
**Date:** 19 January 2026
