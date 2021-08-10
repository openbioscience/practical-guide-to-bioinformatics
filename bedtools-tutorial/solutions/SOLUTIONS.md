# Solutions to `bedtools` tutorial

## Exercise 1: Find non-exons

```console
$ bedtools complement -i exons.bed -g genome.txt > notexons.bed
```

## Exercise 2: Find exons in 500kb regions

```console
$ bedtools makewindows -g genome.txt -w 500000 > windows.bed
$ bedtools coverage -a windows.bed -b exons.bed -counts > windows.exons.bedg
```

## Exercise 3: Finding flanking splice sites

```console
$ bedtools flank -i exons.bed -g genome.txt -b 2 > splice-sites.bed
```

## Exercise 4: Find overlapping exons

```console
$ grep "Enhancer" hesc.chromHmm.bed > hesc.enhancers.bed
$ bedtools intersect -a exons.bed -b hesc.enhancers.bed -f 1.0 > overlap.bed
$ wc -l < overlap.bed > count
```

## Exercise 5: Calculate Jaccard statistics

```console
$ grep "Enhancer" hesc.chromHmm.bed > hesc.enhancers.bed
$ bedtools jaccard -a cpg.bed -b hesc.enhancers.bed > jaccard.enhancers.txt
$ grep "Promoter" hesc.chromHmm.bed > hesc.promoters.bed
$ bedtools jaccard -a cpg.bed -b hesc.promoters.bed > jaccard.promoters.txt
```
