# Practical Guide to Bioinformatics Tools

## Recommended Order
TODO: Add image of recommended prereqs

**Note:** Tutorials are presented in the recommended order of completion.

---

## FASTA file format

## GenBank and RefSeq

**GenBank**: _Uncurated database of nucleic acid and protein sequences from labs around the world._
**RefSeq**: _Curated DNA, mRNA, and protein sequences._

- The difference between GenBank and RefSeq is that GenBank is not curated.

### Tutorials
- [GenBank Sample Record with explanations](https://www.ncbi.nlm.nih.gov/Sitemap/samplerecord.html).

### Notes
- Updates denoted by increment to the numeric version after the decimal; e.g. `NM_xxx.2` ([source](https://archive.is/W6CyS))
- [NCBI Handbook, Chapter 18: The RefSeq Database](https://www.ncbi.nlm.nih.gov/books/NBK21091/)

---

## Gene

_Database of genes integrated information from multiple data sources._

- [Documentation for the Gene Database](https://www.ncbi.nlm.nih.gov/books/NBK3839/)
  - [Documentation on Advanced Search Queries](https://www.ncbi.nlm.nih.gov/books/NBK3841/)


---

## Entrez: NCBI Global Database Search

### Programmatic Access: Entrez API
- [Entrez Programming Utilities (E-utilities)](https://www.ncbi.nlm.nih.gov/books/NBK25501/)
  - [Entrez Direct: E-utilities on the Unix Command Line](https://www.ncbi.nlm.nih.gov/books/NBK179288/)

---

## dbVar

---

## bedtools

_Genome feature manipulation tool._

Developed by the [Quinlan Lab at the University of Utah](http://quinlanlab.org/).

### Tutorials
1. [Description of the BED (Browser Extensible Data) file format.](http://genome.ucsc.edu/FAQ/FAQformat.html#format1)
    - BED files provide a flexible way to define the data lines that are displayed in an genome annotation track.
2. [Introduction to bedtools (sandbox.bio)](https://sandbox.bio/tutorials/?id=bedtools-intro)


---

## SAM/BAM (`.sam`, `.bam`) file format

_Sequence alignment/mapping file format._

---

## bowtie2

_Aligner._

- Output
  - Generates SAM files

- [Github repository](https://github.com/BenLangmead/bowtie2)

---

## samtools

- [Github repository](https://github.com/samtools/samtools)

---

## VCF/BCF (`.vcf`, `bcf`) file format

_Variant call format (and binary counterpart) files are used to describe sequence variations in genomic data._

- Types of variations include
  - Single nucleotide variants
  - Insertions
  - Deletions

- [learn.gencore.bio.nyu.edu: VCF](https://learn.gencore.bio.nyu.edu/ngs-file-formats/vcf-format/)

---

## bcftools

- [Github repository](https://github.com/samtools/bcftools)

---

## General Feature Format (GFF3) file format

- [learn.gencore.bio.nyu.edu: GFF3](https://learn.gencore.bio.nyu.edu/ngs-file-formats/gff3-format/)
_
---
