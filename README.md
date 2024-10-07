# sRNAminer
a Multifunctional Toolkit for Next Generation Sequencing Small RNA Data Mining

sRNAminer, a stand-alone efficient toolkit that involves all common sRNA analysis functions with a user-friendly interface. Notably, sRNAminer is a platform-independent software that can be run under all operating systems 【Windows, MacOS and Linux】.

The functions of sRNAminer are divided into three main parts. (1) Data pre-processing. This part is separated into five steps. a. Adapter trimming. b. Sequence Collapsing. Merging the repetitive sequences. c. Data cleaning. Removing the ncRNA (rRNA, tRNA, snoRNA, snRNA) and organelle fragments. d. Mapping. Reads are mapped to the reference genome. (2) sRNA identification and expression calculation. In detail, miRNA and hc-siRNA identification follows the well-established criteria. phasiRNA is based on p-value and phasing score which are developed in previous studies. Digital expression of miRNA and phasiRNA are calculated by reads per 10 million (RP10M). (3) Other common sRNA analysis functions. sRNA target analysis, sRNAloci identification and expression calculation, trigger analysis, and degradome analysis are involved. All the sRNA analysis methods were coded from scratch using Java, except for the degradome analysis, which was cited from the previous study (Kakrana et al. 2014)

## Download and Installation
sRNAminer is a platform-independent software that can be run under all operating systems. lt is available to users at https://github.com/kli28/sRNAminer/releases
<p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><span property="dct:title">sRNAminer</span> is licensed under <a href="http://creativecommons.org/licenses/by-nc-sa/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-NC-SA 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/sa.svg?ref=chooser-v1"></a></p>

For the command-line version, users can download it from conda:
```shell
conda install srnaminer
```
## Instruction
https://www.yuque.com/u758713/at2327 (Recommend)
or
PDF in the releases
## Q&A
1. Why all the miRNAs in result file are labeled "Novel"
This may be because your blast software is not running successfully, try downloading a stable version of blast.
```shell
conda install blast=2.12
```
