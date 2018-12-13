# Using Targeted Sequencing to Further Cancer Diagnostics
1. [Introduction](#1)<br>
2. [Overivew of Methods](#2)<br>
3. [Overview of Tools](#3)<br>
	a. [Whole Genome Sequencing](#31)<br>
	b. [Whole Exome Sequencing](#32)<br>
	c. [CAPP-Seq](#33)<br>
	d. [TAm-Seq](#34)<br>
4. [Applications & Future Use](#4)<br>
5. [Data Tables & Figures](#5)<br>




## Introduction<a name="1"></a>

The field of cancer diagnostics has experienced tremendous growth and technical developments over the past decade. The advent of high throughoupt sequencing technologies coupled with high-specificity screening methods is enabling the discovery of new biomarkers and potential early disease diagnosis of patients. [1] With early diagnosis comes a variety of benefits for the patient including increased treatment options and higher overall survival rate. For colon cancer ,there is a 91% 5-year survival rate when diagnosed early versus only 11% survival rate if it is caught late and has spread to other organs. [4] Unfortunately, current diagnosis options such as tissue biopsies, endoscopy, or radiology are often invasive to patients. In addition, tissue biopsies only provide a snapshot of the mutations in a patient.

In this chapter, we will be introducing the use of sequencing technologies to analyze liquid biopsy based cancer samples. Early studies in 1977 revealed a high level of cell free DNA and circulating tumor DNA in cancer patient plasma. Liquid biopsy based diagnostics how to solve the invasive and costly drawbacks of tissue biopsy while serving as a highly specific predictor of cancer. Liquid biopsy aims to detect cancer mutations within the plasma, provide early screening options for these mutations, and monitor these mutations over time to assess tumor burden and treatment effectiveness.

Liquid Biopsy Overview: https://www.ncbi.nlm.nih.gov/pubmed/29747380


## Overivew of Methods<a name="2"></a>

Liquid vs Tissue Biopsy: <br>
![](./CTCvsctDNA.jpg) <br>
[Figure 1](https://www.sciencedirect.com/science/article/pii/S2001037018300060#s0030).
** Comparison of the types of mutations and analysis that can be conducted with tissue & liquid based biopsy techniques. **


#### Whole Genome Sequencing (WGS): <a name="31"></a>



#### Whole Exome Sequencing (WES) :<a name="32"></a>

CAPP-Seq Workflow: <br>
![](./CAPP-Seq.png)<br>
[Figure 2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4016134/figure/F1/). 
** Population level analysis is conducted to identify a set of selector regions for CAPP-Seq. Both tissue and liquid biopsy sample are analyzed to identify and validate personalized cancer markers. **

#### CAPP-Seq:<a name="33"></a>
Cancer Personalized Profiling by Deep Sequencing (CAPP-Seq) is a highly sensititve and economical method to quantify ctDNA. In general, ctDNA levels are highly correlated with tumor volume and can provide earlier treatment response assessment compared to radiographic approaches. In non-small cell lung cancer patients, ctDNA was detected in 100% of stage II-IV tumors and 50% of stage I tumors. The CAPP-Seq technique requires designing a "selector" of biotinylated DNA oligonucleotides that target recurrently mutated regions in the cancer of interest. The selector panel is often optimized using WES data and other intron breakpoints to best span the mutated areas. CAPP-Seq can be further applied to disease stage monitoring as it can predict tumor stage progression via ctDNA analysis with a relatively high degree of sensitivity and specificity. [3]


Experimentally, it is possible to use CAPP-Seq across different time points to understand how the allele frequencies of different mutations are changing in response to treatment. This approach requires analyzing both ctDNA and germline DNA as a baseline to compare the variants. Mutations that tend to increase in frequency may be experiencing selective pressure and targeting these mutations can signficantly reduce disease progression. [3]

TAm-Seq Workflow:
![](./TAm-SeqMonitoring.jpg)<br>
[Figure 3](http://stm.sciencemag.org/content/scitransmed/4/136/136ra68/F4.large.jpg).
** The allele frequencies of mutations in breast cancer patients are monitored to view their relationship with time and treatment. **


#### TAm-Seq:
TAm-Seq is a method for tagged-amplicon deep sequencing that allows for the identification of cancer mutations in circulating DNA present at allele frequencies as low as 2%. With a sensitivity and specificity of over 97%, TAm-Seq can be used to monitor tumor dynamics, track mutations, and identify the origin of relapse in a patient with multiple primary tumors. [2] The image below shows the progression of a disease at various time points where the allele frequencies are being measured by TAm-Seq. PR indicates partial response, SD is stable disease, and PD is progressive disease.




The TAm-Seq method uses a combination of short amplicons, two-step amplification, sample barcode sequences, and high-throughput PCR. Because the amplicons are short, this method effectively amplifies even small amounts of fragmented DNA such as are present in circulating DNA. The two-step amplification permits extensive primer multiplexing that enables the amplification and sequencing of sizeable genomic regions by tiling short amplicons without loss of fidelity or efficiency. Duplicate sequencing of each sample is used to avoid false positives stemming from PCR errors. Sample barcodes and high-throughput PCR reduce the per-sample costs to a range where this may be widely applicable. Preparing TAm-Seq libraries for sequencing from 48 samples takes less than 24 hours and involves only few hours of hands-on time. New platforms for massively parallel sequencing allow for fast turnaround times, which make this approach practical in a clinical setting. [2]

We therefore applied TAm-Seq as a generic tool to measure changes in the frequency of ctDNA over time. We studied serial plasma samples collected during follow-up and treatment of two patients with relapsed HGSOC, collected during 104 and 273 days of follow-up and treatment, respectively. Frequencies of mutant TP53 alleles were measured by TAm-Seq and in parallel by digital PCR using a mutation-specific probe. The two methods of quantification had excellent agreement. Mutant AFs in plasma of ovarian cancer patients reflected well the clinical course of the disease compared to the serum marker CA125, showed marked decrease when systemic treatment was initiated, and increased in parallel to disease progression.

Prototypic example where the AF's of 10 different mutations in a patient with metastatic breast cancer all sharply decline upon onset of the chemotherapy, but increase after termination of the therapy. By monitoring the AF of common mutations amongst patients with different disease subsets, it may be possible to generate more personalized treatment options.

https://www.ncbi.nlm.nih.gov/pubmed/22649089


## Future Applications & <a name="4"></a> 


## Industry Overview <a name="5"></a> 
The cancer diagnostics industry is expected to reach a net worth of approximately 232.7 billion USD by 2025. The market of individuals who could benefit from more accurate diagnostics increases annually as the National Cancer Institute estimates approximately 14 million new cases a year. There are a variety of companies developing technologies to further cancer diagnostics. GRAIL uses high through-put sequencing to understand cancer causing mutations while Freenome uses machine learning to predict immune response that are results of cancer development. 




## Data Tables & Figures <a name="6"></a> 
<table>
 <tbody>
    <tr>
        <th>Attribute / Parameter </td>
        <th>Whole Genome Sequencing (WGS) </td>
        <th>Whole Exome Sequencing (WES)</td>
        <th>Targeted Sequencing</td>
    </tr>
    <tr>
        <td> Information Level </td>
        <td> Everything </td>
        <td> Genes </td>
        <td> User Defined </td>
    </tr>
    <tr>
        <td> Cost Per Sample </td>
        <td> $5000 </td>
        <td> $2000 </td>
        <td> $200 </td>
    </tr>
    <tr>
        <td> Low Frequency Mutation Detection </td>
        <td> Not Possible </td>
        <td> Not Likely </td>
        <td> Yes </td>
    </tr>
    <tr>
        <td> DNA Input Amount </td>
        <td> 1 ug </td>
        <td> 100 - 200 ng </td>
        <td> 10 ng </td>
    </tr>
    <tr>
        <td> # of Samples in Parallel </td>
        <td> 1 </td>
        <td> 2 </td>
        <td> 96 </td>
    </tr>
 </tbody>
</table>



## References <a name="7"></a> 
[1] “Biomarkers.” Canary Foundation, www.canaryfoundation.org/canary-science/science/biomarkers/. <br>

[2] Forshew, Tim. “Noninvasive Identification and Monitoring of Cancer Mutations by Targeted Deep Sequencing of Plasma DNA.” Science Translational Medicine, American Association for the Advancement of Science, 30 May 2012, stm.sciencemag.org/content/4/136/136ra68.long. 

[3] Newman, Aaron M, and Maximilian Diehn. “An Ultrasensitive Method for Quantitating Circulating Tumor DNA with Broad Patient Coverage.” Nature News, Nature Publishing Group, 6 Apr. 2014, www.nature.com/articles/nm.3519.

[4] “Understanding Statistics Used to Guide Prognosis and Evaluate Treatment.” Cancer.Net, 11 Aug. 2018, www.cancer.net/navigating-cancer-care/cancer-basics/understanding-statistics-used-guide-prognosis-and-evaluate-treatment.<br>




