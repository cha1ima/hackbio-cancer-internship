<a id="_6agy3xqjct9u"></a>**Gene Expression Patterns in Glioblastoma: Heatmap Visualization and Pathway Enrichment Analysis**

@Hackbio @slack

 _Authors:_

<!--[if !supportLists]-->●      <!--[endif]-->Chaima BenMohamed

<!--[if !supportLists]-->●      <!--[endif]-->Charlotte Chinwendu Iwuji

<!--[if !supportLists]-->●      <!--[endif]-->Chigozie Nkwocha

<!--[if !supportLists]-->●      <!--[endif]-->Igwebuike Vivian

<!--[if !supportLists]-->●      <!--[endif]-->Opeyemi De Campos

<!--[if !supportLists]-->●      <!--[endif]-->Reem  Atawia


# <a id="_18hap44o051h"></a> 

# <a id="_hpl2mx8rc74"></a> 

****


# <a id="_uexrg32exz33"></a> 

# <a id="_ucx8kgj2u9ge"></a>Introduction

Glioblastoma, the most prevalent primary malignant brain tumor in adults, constitutes around 50% of such cases. It affects approximately 3-4 individuals per 100,000 and has a median survival of 14-20 months, varying with the patient's age at diagnosis. Early diagnosis involves surgical resection, stereotactic tumor biopsy, or medical imaging. Current treatment includes surgical resection, radiotherapy, and chemotherapy (Brown et al., 2022). Ongoing research employs omics techniques to better understand the disease's pathogenesis and metabolic pathways (Gilard et al., 2021). This report analyses differentially expressed genes in glioblastoma using RNA-seq data, available [here](https://raw.githubusercontent.com/HackBio-Internship/public_datasets/main/Cancer2024/glioblastoma.csv), and conducts pathway enrichment analysis to elucidate the biological processes involved in its pathogenesis.****


# <a id="_of07d0c8m5gw"></a>Protein with unfavorable prognosis in GBM

As shown in Figure 1, many genes are known to cause the pathogenesis of glioblastoma. Amongst this is the EGF (Epidermal growth factor) gene. This gene encodes the Epidermal Growth Factor Receptor (EGFR) protein which is involved in cell signaling pathways that control cell division and survival. The** **EGFR protein, also known as HER1 or ErbB1, is part of the ErbB receptor family and has a tyrosine kinase activity (Brosseau _et al_., 2015).

Mutations in this gene can lead to the overexpression of the EGFR protein resulting in an abnormal or uncontrolled cellular proliferation. In EGFR-driven glioblastoma, the majority of mutations are missense mutations on the EGFRvII and EGFRvIII variants. One other variant, the EGFRx variant, which has deleted exons 2–14 and lacks a binding domain, is crucial for tumor growth and development in glioblastoma xenografts (Huang _et al_., 2023, Chen _et a_l., 2016, Singh _et al_., 2023).

<!--[if gte vml 1]><v:shapetype id="_x0000_t75" coordsize="21600,21600"
 o:spt="75" o:preferrelative="t" path="m@4@5l@4@11@9@11@9@5xe" filled="f"
 stroked="f">
 <v:stroke joinstyle="miter"/>
 <v:formulas>
  <v:f eqn="if lineDrawn pixelLineWidth 0"/>
  <v:f eqn="sum @0 1 0"/>
  <v:f eqn="sum 0 0 @1"/>
  <v:f eqn="prod @2 1 2"/>
  <v:f eqn="prod @3 21600 pixelWidth"/>
  <v:f eqn="prod @3 21600 pixelHeight"/>
  <v:f eqn="sum @0 0 1"/>
  <v:f eqn="prod @6 1 2"/>
  <v:f eqn="prod @7 21600 pixelWidth"/>
  <v:f eqn="sum @8 21600 0"/>
  <v:f eqn="prod @7 21600 pixelHeight"/>
  <v:f eqn="sum @10 21600 0"/>
 </v:formulas>
 <v:path o:extrusionok="f" gradientshapeok="t" o:connecttype="rect"/>
 <o:lock v:ext="edit" aspectratio="t"/>
</v:shapetype><v:shape id="image4.png" o:spid="_x0000_i1031" type="#_x0000_t75"
 style='width:451.2pt;height:208.2pt;visibility:visible;mso-wrap-style:square'>
 <v:imagedata src="file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png"
  o:title=""/>
</v:shape><![endif]--><!--[if !vml]-->![](https://github.com/cha1ima/hackbio-cancer-internship/blob/main/Stage%202/Images/Figure%201.png?raw=true)<!--[endif]-->
![Figure 1](https://github.com/cha1ima/hackbio-cancer-internship/blob/main/Stage%202/Images/Figure%201.png?raw=true)
**_Figure 1: _**_EGFR signaling and related pathways in cancer involve gene products that transmit signals from the cell surface to the nucleus, mediated by EGFR._


# <a id="_f5ecxpz5n8r7"></a>Data Preprocessing and Analysis

The downloaded dataset contains over 500 gene expressions from 10 patients. This data was explored and preprocessed for analysis. Data exploration and preprocessing steps include data visualization to visualize the pattern in gene expression levels using a heatmap. Heatmaps showed clusters from genes and samples alone and both samples and genes together.

Heatmaps rely on color to represent the magnitude of values, so appropriate color selection ensures that high, low, and medium values are clearly distinguishable. The **diverging color palette** uses colors to show how values deviate from low to high with a midpoint, while the **sequential color palette **highlights how data points move from an increasing continuous value in a gradient. Appropriate diverging or sequential colours aid colour-blind friendliness.


## <a id="_it1sgdtox51o"></a>Data Visualization

**Genes only**

<!--[if gte vml 1]><v:shape id="image3.png" o:spid="_x0000_i1030"
 type="#_x0000_t75" style='width:451.2pt;height:351pt;visibility:visible;
 mso-wrap-style:square'>
 <v:imagedata src="file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image003.png"
  o:title=""/>
</v:shape><![endif]--><!--[if !vml]-->![](file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image004.jpg)<!--[endif]-->

**_Figure 2: _**_Heatmap showing clusters on genes alone_

\


**_ _**

**Both genes and samples**

<!--[if gte vml 1]><v:shape id="image2.png" o:spid="_x0000_i1029"
 type="#_x0000_t75" style='width:418.2pt;height:325.2pt;visibility:visible;
 mso-wrap-style:square'>
 <v:imagedata src="file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image005.png"
  o:title=""/>
</v:shape><![endif]--><!--[if !vml]-->![](file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image006.jpg)<!--[endif]-->

**_Figure 3: _**_Heatmap showing clusters on genes and samples_****

** **

** **

** **

** **

** **

** **

** **

** **

** **

** **

** **

**Samples only**

<!--[if gte vml 1]><v:shape id="image6.png" o:spid="_x0000_i1028"
 type="#_x0000_t75" style='width:430.8pt;height:307.2pt;visibility:visible;
 mso-wrap-style:square'>
 <v:imagedata src="file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image007.png"
  o:title=""/>
</v:shape><![endif]--><!--[if !vml]-->![](file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image008.jpg)<!--[endif]-->

**_Figure 4: _**_Heatmap showing clusters on samples alone_

Based on the pattern seen in Figure 4, samples with ‘2005’ in their IDs were assigned to one group and others to another group, and these groups were used as metadata for gene expression analysis.


## <a id="_epubdsw9ew7s"></a>Data Analysis and Results

**Differentially expressed genes**

To determine differentially expressed genes, the t-statistical test was used to compare if the mean gene expression** **levels between groups are statistically significant at a 5% significance level. Next, the log2 fold change for each gene between groups was obtained. Using a cutoff of absolute log2 fold change of 1.5, differentially expressed genes were selected for genes with absolute fold changes greater than 1.5, where upregulated genes had log2 fold changes greater than 1.5 and downregulated genes less than -1.5.

From our result, 10 upregulated and 2 downregulated genes were obtained. Figure 5 is a volcano plot showing differentially expressed genes (in green and coral colors).

<!--[if gte vml 1]><v:shape id="image7.png" o:spid="_x0000_i1027"
 type="#_x0000_t75" style='width:431.4pt;height:307.8pt;visibility:visible;
 mso-wrap-style:square'>
 <v:imagedata src="file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image009.png"
  o:title=""/>
</v:shape><![endif]--><!--[if !vml]-->![](file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image010.jpg)<!--[endif]-->

**_Figure 5: _**_Volcano Plot of Glioblastoma dataset (Horizontal axis represents log2-fold change, and the vertical axis represents adjusted p-value)._

**Functional Enrichment Analysis**

Functional enrichment analysis was performed with ShinyGO using the upregulated and downregulated gene IDs. According to biological processes, three enriched pathways were identified for upregulated genes, namely: Glutathione derivative metabolic process, Glutathione derivative biosynthetic process, and Proteolysis, while five enriched pathways were identified for downregulated genes, namely: Ribosomal small subunit assembly, Maturation of SSU-rRNA from tricistronic rRNA transcript (SSU-rRNA 5), Maturation of SSU-rRNA , Ribosomal Small Subunit Biogenesis and Ribosome assembly as shown in figure 6 and figure 7 below with pvalue < 0.05 and log2FC < -1.5, for downregulation and pvalue < 0.05 and log2FC > 1.5, for upregulation.

<!--[if gte vml 1]><v:shape id="image5.png" o:spid="_x0000_i1026"
 type="#_x0000_t75" style='width:451.2pt;height:313.2pt;visibility:visible;
 mso-wrap-style:square'>
 <v:imagedata src="file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image011.png"
  o:title=""/>
</v:shape><![endif]--><!--[if !vml]-->![](file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image012.jpg)<!--[endif]-->

**_Figure 6: _**_Top five biological processes for downregulated genes._

<!--[if gte vml 1]><v:shape id="image1.png" o:spid="_x0000_i1025"
 type="#_x0000_t75" style='width:432.6pt;height:299.4pt;visibility:visible;
 mso-wrap-style:square'>
 <v:imagedata src="file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image013.png"
  o:title=""/>
</v:shape><![endif]--><!--[if !vml]-->![](file:///C:/Users/MONTA/AppData/Local/Temp/msohtmlclip1/01/clip_image014.jpg)<!--[endif]-->

**_Figure 7_**_: Top three biological processes pathways for upregulated genes._

Figures 6 and 7 are **lollipop charts** showing the top biological processes for downregulated and upregulated genes, respectively. The dots show the number of genes in each biological process and the colors of the line show their fold enrichment scores.

**Top 3 Upregulated enriched pathways according to biological processes**

**1. Glutathione derivative metabolic proc.**

**Description:** This pathway involves the metabolism of glutathione derivatives, crucial for neutralizing reactive oxygen species (ROS) and protecting cells from oxidative stress. In cancer, changes in the glutathione system contribute to tumor initiation, progression, and treatment response. While glutathione detoxifies carcinogens in healthy cells, elevated levels in tumor cells promote growth and resistance to chemotherapy.** **(Kennedy_ et al._, 2020)

**2. Glutathione derivative Bio synthetic proc.**

**Description:** This pathway involves the biosynthesis of glutathione derivatives, essential for detoxification and protection against oxidative damage. In cancer, upregulation of this pathway reflects increased glutathione production to maintain redox balance, helping tumor cells, like in glioblastoma, survive oxidative stress and enhance aggressiveness.(Backos _et al_., 2012)****

**3. Proteolysis**

**Description: **In glioblastoma, increased proteolysis may aid tumor microenvironment remodeling, extracellular matrix degradation, and misfolded protein clearance, helping cancer cells survive stress, avoid apoptosis, and support tumor growth and metastasis. Lysosomal cathepsins regulate protein degradation to maintain proteome balance, but dysregulated activity can be harmful. In tumor cells, certain cathepsins are upregulated, with elevated Cathepsin B activity linked to increased glioblastoma stem cell mobility. (Bischof _et al.,_ 2017)****

**Top 3 Down regulated enriched pathways according to biological processes**

**1. Ribosomal small subunit assembly**

Ribosomal proteins possess both oncogenic and anti-tumor  activities. Increased expression of ribosomal protein S6 ensures stem-cell-like phenotypes in Glioblastoma (Hide _et al., 2022_)

**2. Maturation of SSU-rRNA from tricistronic rRNA transcript (SSU-rRNA 5)**

Ribosomal proteins are linked to various aspects of carcinogenesis, with their extra-ribosomal functions causing negative effects such as cell cycle arrest, apoptosis, and cellular senescence.(Shirakawa_ et al_., 2021)

**3. Maturation of SSU-rRNA : **Ribosomopathies in humans are disorders resulting from genetic defects in ribosomal proteins, rRNAs, or RNA polymerases, causing disabilities and promoting cancer development.(McElreavey _et al._, 2022)

 


# <a id="_o9gzjgtxffh5"></a>REFERENCES

Backos, D.S., Franklin, C.C. and Reigan, P., 2012. The role of glutathione in brain tumor drug resistance. _Biochemical Pharmacology_, 83(8), pp.1005-1012. doi: 10.1016/j.bcp.2011.11.016.

Bischof, J., Westhoff, M.-A., Wagner, J.E., et al., 2017. Cancer stem cells: The potential role of autophagy, proteolysis, and cathepsins in glioblastoma stem cells. _Tumor Biology_, 39(3). doi:10.1177/1010428317692227.

Brosseau, S., Viala, M., Varga, A., Planchard, D., Besse, B. and Soria, J.C., 2015. 3rd generation's TKI in lung cancer non-small cell EGFR-mutated having acquired a secondary T790M resistance. _Bulletin du Cancer_, 102, pp.749–757. doi: 10.1016/j.bulcan.2015.05.001.

Brown, N.F., Ottaviani, D., Tazare, J., Gregson, J., Kitchen, N., Brandner, S., Fersht, N. and Mulholland, P., 2022. Survival outcomes and prognostic factors in glioblastoma. _Cancers_, 14(13). doi: 10.3390/cancers14133161.

Chen, J., Zeng, F., Forrester, S.J., Eguchi, S., Zhang, Z. and Harris, R.C., 2016. Expression and function of the epidermal growth factor receptor in physiology and disease. _Physiological Reviews_. doi: 10.1152/PRV-00030-2015.

Gilard, V., Tebani, A., Dabaj, I., Laquerrière, A., Fontanilles, M., Derrey, S., Marret, S. and Bekri, S., 2021. Diagnosis and management of glioblastoma: A comprehensive perspective. _Journal of Personalized Medicine_, 11(4). doi: 10.3390/jpm11040258.

Hide, T., Shibahara, I., Inukai, M., Shigeeda, R. and Kumabe, T., 2022. Ribosomes and ribosomal proteins promote plasticity and stemness induction in glioma cells via reprogramming. _Cells_, 11(14), p.2142.

Huang, W., Li, J., Zhu, H., Qin, X., Chen, C., Wang, B., Wei, J., Song, Y., Lu, X., Li, Z., et al., 2023. A novel EGFR variant EGFRx maintains glioblastoma stem cells through STAT5. _Neuro-Oncology_, 26, pp.85–99.

Kennedy, L., Sandhu, J.K., Harper, M.E. and Cuperlovic-Culf, M., 2020. Role of glutathione in cancer: From mechanisms to therapies. _Biomolecules_, 10(10), p.1429. doi: 10.3390/biom10101429.

McElreavey, K., Pailhoux, E. and Bashamboo, A., 2022. DHX37 and 46,XY DSD: A new ribosomopathy? _Sexual Development_, 16, pp.194–206.

Singh, S., Barik, D., Lawrie, K., Mohapatra, I., Prasad, S., Naqvi, A.R., Singh, A. and Singh, G., 2023. Unveiling novel avenues in mTOR-targeted therapeutics: Advancements in glioblastoma treatment. _International Journal of Molecular Sciences_, 24, p.14960.

Shirakawa, Y., Ohta, K., Miyake, S., Kanemaru, A., Kuwano, A., Yonemaru, K., Uchino, S., Yamaoka, M., Ito, Y., Ito, N., Hide, T., Shinojima, N., Mukasa, A., Saito, H. and Jono, H., 2021. Glioma cells acquire stem-like characters by extrinsic ribosome stimuli. _Cells_, 10(11), p.2970. doi: 10.3390/cells10112970.
