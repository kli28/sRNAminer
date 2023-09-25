# sRNAminer
a Multifunctional Toolkit for Next Generation Sequencing Small RNA Data Mining

sRNAminer, a stand-alone efficient toolkit that involves all common sRNA analysis functions with a user-friendly interface. Notably, sRNAminer is a platform-independent software that can be run under all operating systems 【Windows, MacOS and Linux】.

The functions of sRNAminer are divided into three main parts. (1) Data pre-processing. This part is separated into five steps. a. Adapter trimming. b. Sequence Collapsing. Merging the repetitive sequences. c. Data cleaning. Removing the ncRNA (rRNA, tRNA, snoRNA, snRNA) and organelle fragments. d. Mapping. Reads are mapped to the reference genome. (2) sRNA identification and expression calculation. In detail, miRNA and hc-siRNA identification follows the well-established criteria. phasiRNA is based on p-value and phasing score which are developed in previous studies. Digital expression of miRNA and phasiRNA are calculated by reads per 10 million (RP10M). (3) Other common sRNA analysis functions. sRNA target analysis, sRNAloci identification and expression calculation, trigger analysis, and degradome analysis are involved. All the sRNA analysis methods were coded from scratch using Java, except for the degradome analysis, which was cited from the previous study (Kakrana et al. 2014)

## Download and Installation
sRNAminer is a platform-independent software that can be run under all operating systems. lt is freely available to **non-commercial** users at https://github.com/kli28/sRNAminer/releases

For the command-line version, users can download it from conda:
```shell
conda install srnaminer
```

