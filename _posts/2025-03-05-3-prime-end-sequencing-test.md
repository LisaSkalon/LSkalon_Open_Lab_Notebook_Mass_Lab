---
layout: post
title: 3'-end sequencing test
category: Library preparation
tags: [ RNA,library,Stylophora]
---

Here, I tested 3'-end libraries sequencing results. 

### Samples

| Sample | Quantity   | 260/280  | 230/280 | RIN     | Tube id
| ------ | ---------- | -------- | ------- | ------- | ------- |
| S1     | 16.3 ng/ul | 1.88     | 0.57    | 8.3     | 1 RNA 16S 06.11 |
| S2     | 17.8 ng/ul | 2.2      | 2.18    | 9.2     | 1.8 RNA 12.11 |

The libraries were constructed 3 times from each sample, pooled together and sequenced. In total, 6 files with raw reads were created:

|  file prefix     |    description    |
| ------ | ----------------------- |
| TM1_S1 | preparation 1, sample 1 |
| TM1_S2 | preparation 1, sample 2 |
| TM2_S1 | preparation 2, sample 1 |
| TM2_S2 | preparation 2, sample 2 |
| TM3_S1 | preparation 3, sample 1 |
| TM3_S2 | preparation 3, sample 2 |

### Initial fastqc results
Initial quality was accessed with fastqc. 

![General stats](https://github.com/LisaSkalon/LSkalon_Open_Lab_Notebook_Mass_Lab/blob/master/images/general.stat.before.png)  
![Per base quality](https://github.com/LisaSkalon/LSkalon_Open_Lab_Notebook_Mass_Lab/blob/master/images/fastqc_per_base_sequence_quality_plot.before.png)  
![Adaptors](https://github.com/LisaSkalon/LSkalon_Open_Lab_Notebook_Mass_Lab/blob/master/images/fastqc_adapter_content_plot.before.png)  

High duplication level and high polyA/adaptor content, as well as failed GC-content plot are normal for 3'-end data. Overall, the quality of all samples is good, but the sequencing depth is different, for TM3 it is below 10 million reads.

### Fastqc after trimming
Reads were trimmed with Trimmomatic to get rid of adaptors and polyA + to remove low quality bases (Phred < 30). Reads shorter than 30 bp were discarded.
The number of reads reduced in each sample, but the most dramatical reduction was observed in TM3. 
![General stats](https://github.com/LisaSkalon/LSkalon_Open_Lab_Notebook_Mass_Lab/blob/master/images/general.stat.after.png)  

### STAR mapping to S. pistillata genome

Reads were mapped to S. pistillata reference genome with standard STAR parameters. 

![General stats](https://github.com/LisaSkalon/LSkalon_Open_Lab_Notebook_Mass_Lab/blob/master/images/general.stat.star.png)  
![Mapping stat](https://github.com/LisaSkalon/LSkalon_Open_Lab_Notebook_Mass_Lab/blob/master/images/star_alignment_plot.png)  
![Mapping stat perc](https://github.com/LisaSkalon/LSkalon_Open_Lab_Notebook_Mass_Lab/blob/master/images/star_alignment_plot2.png)  
![Counts](https://github.com/LisaSkalon/LSkalon_Open_Lab_Notebook_Mass_Lab/blob/master/images/star_gene_counts.png)  
![Counts perc](https://github.com/LisaSkalon/LSkalon_Open_Lab_Notebook_Mass_Lab/blob/master/images/star_gene_counts2.png)  
