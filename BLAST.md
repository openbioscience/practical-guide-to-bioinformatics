# BLAST

## Interpreting BLAST output

```console
$ cat lantibiotic.fasta
>lcl|LISX01000003.1_cds_OKJ13746.1_3580 [locus_tag=AMK19_09970] [protein=lantibiotic biosynthesis protein] [protein_id=OKJ13746.1] [location=379245..380294]
ATGACTGACCTGCCGACCACCCCGGACGCCCCCGGCGACTGGCTCGCGCTGCACGTCTTCTACGCGGCCAGCCCGCGCCC
GCTGCTGCTGCAGTGCGTGCGCCCGCTGGTCGCCGAACTCACCGAAGAGGGCCTGCTCGCCGGGCACTTCTTCATCAACT
ACTGGGTGGAGGGCCCGCACCTGCGCCTGCGCCTGCGGCCCGCCACCCCCGAGGCGGCCGAACAGGTCCGCGCACGTGCC
GAGAGCGCCGTCGCCGAGTTCCTGCGCCGCCGCCCCGCGCTCTACCAGGTCGAGGACAGCTTCTTCGCGGAGCTCTACAA
CACCATGTTCGAGCTGGAGTTCACCCTGGAGGAACGCGCCGAACTCGTCGACGCCGACGGGAGGATGAGGCTGCGGGAGA
ACAACACCTTCAGCCGCGAACCGTACGAGCCCGAGTACGGCAAGTACGGCGGCCCGGCCGGCATCGACCTCGCCGAATGG
CACTTCCAGCACTCCAGCGACCTGGTGATCGAAGCCACCCGCACCATGAACCTGCACCTGCGCACCGTGGTGCTGGGCCT
GGCCGCGCAGCTGATGATGACCATGACGGCGTGCTTCCTCCCCGACGAGGACGCCCTGCTGACCTTCCTCGACCGCTACC
ACGCCTTCTGGAACCGCTCGTTCGAAGGCACCAACTACACCGCGCAGCAGGGCTACGACCGCGCCTACACCAGCATGGGC
GACGCCCTGCCGGCCAGGTTCCGGGCGATCCGCGCCGCCGTCGTCGACGGCGCGCCCGAGCGGCTGCCCGCCGTGCTCCG
CGGCTGGGCCGAGCACTGCCTCGACCTGCGCGAGCGCGCCGCCGGGGCGGCGCGCCGCGGCGAACTGGTCTTCCGCTCCT
GGGACGGCGAACGCGACCTGACCGTCACCGACCCCGCCGAGGCGCTGCCGATGCTGCTGTTCCCGTACGCCCACATGACC
AACAACCGGCTGTCGGTGACCGTCCGCGACGAGGCGTTCCTGTCGTACATCCTGGCCCGCGCCCTGCGCGAACCCGCGGT
GGTCTCGTGA
```

Running `blastn` on `lantibiotic.fasta` for taxon (taxid) `2063` yields the following as one of the results:

```
Query  1     MTDLPTTPDAPGDWLALHVFYAASPRPLLLQCVRPLVAELTEEGLLAGHFFINYWVEGPH  180
             MTDL ++PD PGDWLALHVFYAASPRPLLLQCVRPLV EL +EGLLAG+FFINYWVEGPH
Sbjct  1     MTDLSSSPDTPGDWLALHVFYAASPRPLLLQCVRPLVTELADEGLLAGYFFINYWVEGPH  60

Query  181   LRLRLRPATPEAAEQVRARAESAVAEFLRRRPALYQVEDSFFAELYNTMFELEFTLEERA  360
             LRLRLRPA PEAAEQVR RAE+AVAEFLRRRPALYQV DSFFAELYNTMFELEFT +ERA
Sbjct  61    LRLRLRPARPEAAEQVRERAETAVAEFLRRRPALYQVADSFFAELYNTMFELEFTPDERA  120

Query  361   ELVDADGRMRLRENNTFSREPYEPEYGKYGGPAGIDLAEWHFQHSSDLVIEATRTMNLHL  540
             ELV  DGRMRLRENNTFSRE YEPEYGKYGGPAGIDLAEWHFQHSSDLVIEATRTMNLHL
Sbjct  121   ELVGPDGRMRLRENNTFSREEYEPEYGKYGGPAGIDLAEWHFQHSSDLVIEATRTMNLHL  180

Query  541   RTVVLGLAAQLMMTMTACFLPDEDALLTFLDRYHAFWNRSFEGTNYTAQQGYDRAYTSMG  720
             RTVVLGLA QLMMTMTACFLP+ED LL FLDRYHAFWNRSF GTNYTAQQGYDRAY SMG
Sbjct  181   RTVVLGLATQLMMTMTACFLPEEDDLLAFLDRYHAFWNRSFAGTNYTAQQGYDRAYASMG  240

Query  721   DALPARFRAIRAAVVDGAPERLPAVLRGWAEHCLDLreraagaarrgeLVFRSWDGERDL  900
             D LPARFRAIRAA+VD APERLPAVLRGWAEHCL+LRE+AA  ARRGELVFRSWDG RDL
Sbjct  241   DTLPARFRAIRAAIVDRAPERLPAVLRGWAEHCLELREKAAELARRGELVFRSWDGTRDL  300

Query  901   TVTDPAEALPMLLFPYAHMTNNRLSVTVRDEAFLSYILARALREP  1035
             TVTDPAEALPMLLFPYAHMTNNRLSVTVRDEAFLSYILARALREP
Sbjct  301   TVTDPAEALPMLLFPYAHMTNNRLSVTVRDEAFLSYILARALREP  345
```

A useful resource to look at if you don't understand some features of the BLAST output is the [BLAST Frequently Asked Questions page](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=FAQ).

- TODO: low-complexity sequence and lowercase letters.
