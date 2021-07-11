# Practical Guide to Bioinformatics Tools

## Recommended Order
TODO: Add image of recommended prereqs

## RefSeq: curated DNA, mRNA, and protein sequences
- Updates denoted by increment to the numeric version after the decimal; e.g. NM_xxx.2 ([source](https://archive.is/W6CyS))
- [NCBI Handbook, Chapter 18: The RefSeq Database](https://www.ncbi.nlm.nih.gov/books/NBK21091/)

## Gene: gene-specific database integrating multiple data sources
- [Documentation for the Gene Database](https://www.ncbi.nlm.nih.gov/books/NBK3839/)
  - [Documentation on Advanced Search Queries](https://www.ncbi.nlm.nih.gov/books/NBK3841/)

## GenBank and RefSeq:
- The difference between GenBank and RefSeq is that GenBank is not curated.

## Entrez: NCBI Global Database Search

### Programmatic Access: Entrez API
- [Entrez Programming Utilities (E-utilities)](https://www.ncbi.nlm.nih.gov/books/NBK25501/)
  - [Entrez Direct: E-utilities on the Unix Command Line](https://www.ncbi.nlm.nih.gov/books/NBK179288/)

## dbVar

## FAQ

### What is `GCF_[9 digits]` or `GCA_[9 digits]`?
They are [NCBI Genome Assembly accession numbers](https://support.nlm.nih.gov/knowledgebase/article/KA-03451/en-us). GenBank assemblies are given the prefix of `GCA`, while RefSeq assemblies are given the `GCF` prefix.

### What are all these "accession number" prefixes?
|Prefix|Database|Meaning|
|:-----|:-------|:------|
|nsv|dbVar|variant region (sv = structural variant), submitted to NCBI|
|nssv|dbVar|variant call (ssv = supporting structural variant), submitted to NCBI|
|esv|dbVar|variant region, submitted to EBI|
|essv|dbVar|variant call, submitted to EBI|
|dsv|dbVar|variant region, submitted to DDBJ|
|dssv|dbVar|variant call, submitted to DDBJ|
|GCA|GenBank|Genome Assembly|
|GCF|RefSeq|Genome Assembly|

