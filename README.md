# hse_hw3_chromhmm
[Google Colab](https://colab.research.google.com/drive/1somkhIp5qXtbhXKXoU25cMucevZ1TUEj?usp=sharing)
## Histone modifications
**Histone Modification** | **File** | 
------------ | ------------- | 
H2az | wgEncodeBroadHistoneK562H2azStdAlnRep1.bam
H3k4me3| wgEncodeBroadHistoneK562H3k4me3StdAlnRep1.bam
H3k9me1|wgEncodeBroadHistoneK562H3k9me1StdAlnRep1.bam
H4k20me1|wgEncodeBroadHistoneK562H4k20me1StdAlnRep1.bam
H3k27ac|wgEncodeBroadHistoneK562H3k27acStdAlnRep1.bam
H3k36me3|wgEncodeBroadHistoneK562H3k36me3StdAlnRep1.bam
H3k79me2|wgEncodeBroadHistoneK562H3k79me2StdAlnRep1.bam
H3k9ac|wgEncodeBroadHistoneK562H3k9acStdAlnRep1.bam
H3k27me3|wgEncodeBroadHistoneK562H3k27me3StdAlnRep1.bam
H3k4me1|wgEncodeBroadHistoneK562H3k4me1StdAlnRep1.bam
## Images from ChromHMM
![emissions_10](https://user-images.githubusercontent.com/55647212/160098882-eafea2d5-8b2a-46ba-97e6-01b571ff3158.png)

![K562_10_overlap](https://user-images.githubusercontent.com/55647212/160099030-ede29cc8-754c-4e79-b320-24fb53647c4d.png)

![K562_10_overlap](https://user-images.githubusercontent.com/55647212/160098918-c0903035-a1f3-4960-a126-07a520690eae.png)

![K562_10_RefSeqTES_neighborhood](https://user-images.githubusercontent.com/55647212/160099186-af9ce47a-9bb1-40fa-ab2a-1f8554f70ccc.png)

![K562_10_RefSeqTSS_neighborhood](https://user-images.githubusercontent.com/55647212/160099207-87ae6ce9-aea1-4d79-817f-744fb4d17c52.png)

![transitions_10](https://user-images.githubusercontent.com/55647212/160098952-d53cd380-d06c-43de-af80-fad11bcffe31.png)
## States table
**Epigenetic type** | **Epigenetics features** | **Associated Histone Modification** | **State**
------------ | ------------- | ------------- | ------------- 
1 | большой процент в TSS и TES, по расположению (см. GATA2), там 1 находится и в начале и в конце (то есть TSS, TES)| H3k79me2, H3k4me3, H3k9ac | insulator
2 | большой процент в CpG islands, Exon и TSS и находится иногда в начале генома, иногда в exon (см. CD19)| H3k4me3, H3k9ac, H2az | возможно, promoter, [Sharifi-Zarchi, A., Gerovska, D., Adachi, K. et al. (2017)](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-017-4353-7#citeas)
3 | находится в начале гена (chr1) | H3k4me1, H2az | poised promoter, [Bae, S., & Lesch, B. J. (2020)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7214686/)
4 | присутствует в lamina | H2az| repressed heterochromatin
5 | большой процент в TES, находится как в exons, так и в introns(см.CD19) | H3k4me1 | transcriptional elongation
6 | большой процент в RefSeqGene, находится в introns | H3k79me2 | skipping exons, [Li, T., Liu, Q., Garza, N. et al. (2018)](https://genomemedicine.biomedcentral.com/articles/10.1186/s13073-018-0538-1#citeas)
7 | большой процент в RefSeqGene, находится в exons | H3k79me2 | skipping exons, [Li, T., Liu, Q., Garza, N. et al. (2018)](https://genomemedicine.biomedcentral.com/articles/10.1186/s13073-018-0538-1#citeas)
8 | большой процент в TES, иногда покрывает большие участки гена, включая exons и introns (см. TP53) | H3k36me3 | transcriptional elongation, [Kimura, H. (2013)](https://www.nature.com/articles/jhg201366.pdf?origin=ppub)
9 | большой процент во всем геноме, находится в самом начале гена, поэтому похож на promoter, но также большой процент в lamina | NA | возможно, promoter
10 | большой процент во всем геноме, находится в самом начале гена, похож на promoter | NA | возможно, promoter
## Images from USCS Genome Browser
<img width="800" alt="Screen Shot 2022-03-25 at 13 11 59" src="https://user-images.githubusercontent.com/55647212/160101360-d5c7049f-16d7-42e8-8aeb-cacb603241e7.png"> |<img width="800" alt="Screen Shot 2022-03-25 at 13 03 55" src="https://user-images.githubusercontent.com/55647212/160100198-1061bf63-d103-4756-a8e8-92e2eaf43ee1.png">
