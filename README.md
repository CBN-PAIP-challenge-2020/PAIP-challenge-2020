# PAIP-challenge-2020

## Background

CRC develops as a result of the accumulation of genetic and epigenetic alterations and is known as a heterogeneous disease entity with three molecular carcinogenesis pathways and two morphologic multistep pathways. The molecular subtypes of CRC exhibit different responses to adjuvant therapy, which may be responsible for differences in subtype-specific survival. Three molecular carcinogenesis pathways have been identiﬁed: (1) chromosomal instability (CIN), (2) microsatellite instability (MSI), and (3) CpG island methylator phenotype (CIMP) or epigenetic instability pathways. **In this challenge, we will focus on MSI detecting in cases of CRC.**

MSI is a condition of genome-wide alterations in the number of repeat nucleotide(s) caused by a defective DNA mismatch repair by epigenetic inactivation of MLH1 gene or  germline mutations in mismatch repair genes. The microsatellite status of each tumor was **determined by the evaluation of five microsatellite markers: D2S123, D5S346, D17S250, BAT25, and BAT26.** The MSI status was classified as follows:

- MSI-High (MSI-H; instability at ≥ 2 microsatellite markers)
- MSI-Low (MSI-L; instability at 1 marker)
- MSI-Stable (MSS; microsatellite stable or no instability)

MSI-H in CRCs is significantly associated with a better prognosis but does not show benefit from 5-fluorouracil-based adjuvant chemotherapy. Moreover, recent evidence has indicated that MSI-H is a significant predictor of a positive response to immunotherapy using an immune checkpoint blockade in solid tumors. Therefore, the pathological reporting of MSI status is strongly recommended for all surgically resected CRC cases. In clinical practice, however, not every patient is tested for MSI because this requires additional genetic or immunohistochemical tests. By developing these MSI-H classification algorithms, prognoses and responses to immune checkpoint blockade therapy can be predicted simply by using digitally scanned slide images without additional time and cost required for the evaluation of microsatellite markers.

## TASK : MSI-High Classification in Colorectal Cancer

**Notification**  : The **MSI-High(MSI-H) classification is the main task**, which has first priority consideration in the challenge evaluation, **while segmentation is a mandatory task for this challenge.** Therefore, all participants who want to make **a submission need to enclose the result of the MSI-H prediction and segmentation of the whole tumor area.**

## PAIP2019 Results
- Task 1 : Tumor Segmentation
'''html
 <tbody><tr style="height: 17.4pt;">
  <td class="xl66" style="text-align: left; height: 17.4pt; width: 53pt;"><b>Rank</b></td>
  <td class="xl67" style="text-align: left; width: 232pt;"><b>Team Name</b></td>
  <td class="xl67" style="text-align: left; width: 227pt;"><b>Affiliation</b></td>
  <td class="xl68" style="text-align: left; width: 208pt;"><b>Score</b></td>
 </tr>
 <tr style="height: 34.8pt;">
  <td class="xl69" style="height: 34.8pt; width: 53pt;">1</td>
  <td class="xl70" style="width: 232pt;">Hyun
  Jung&nbsp;</td>
  <td class="xl70" style="width: 227pt;">Frederick
  National Laboratory for Cancer Research&nbsp;</td>
  <td class="xl71" style="width: 208pt;">0.788987</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl69" style="height: 17.4pt; width: 53pt;">2</td>
  <td class="xl70" style="width: 232pt;">Team Sen</td>
  <td class="xl70" style="width: 227pt;">Sichuan
  University</td>
  <td class="xl71" style="width: 208pt;">0.777215</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl72" style="height: 17.4pt; width: 53pt;">3</td>
  <td class="xl73" style="width: 232pt;">Team
  MIRL-IITM</td>
  <td class="xl73" style="width: 227pt;">Indian
  Institute of Technology Madras</td>
  <td class="xl74" style="width: 208pt;">0.750333</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl75" style="height: 17.4pt; width: 53pt;">4</td>
  <td class="xl73" style="width: 232pt;">Team
  Damo AIC</td>
  <td class="xl73" style="width: 227pt;">Alibaba
  - alicloud&nbsp;</td>
  <td class="xl74" style="width: 208pt;">0.671778</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl75" style="height: 17.4pt; width: 53pt;">5</td>
  <td class="xl73" style="width: 232pt;">Team
  QuIIL</td>
  <td class="xl73" style="width: 227pt;">Sejong
  University</td>
  <td class="xl74" style="width: 208pt;">0.665227</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl75" style="height: 17.4pt; width: 53pt;">6</td>
  <td class="xl73" style="width: 232pt;">Team
  CUHK-Med</td>
  <td class="xl73" style="width: 227pt;">The
  Chinese University of Hong Kong</td>
  <td class="xl74" style="width: 208pt;">0.662454</td>
 </tr>
 <tr style="height: 34.8pt;">
  <td class="xl75" style="height: 34.8pt; width: 53pt;">7</td>
  <td class="xl73" style="width: 232pt;">Team
  DAISYlab@UKE</td>
  <td class="xl73" style="width: 227pt;">University
  Medical Center Hamburg-Eppendorf (UKE)</td>
  <td class="xl74" style="width: 208pt;">0.65962</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl75" style="height: 17.4pt; width: 53pt;">8</td>
  <td class="xl73" style="width: 232pt;">Team
  COSYPath</td>
  <td class="xl73" style="width: 227pt;">Icahn
  School of Medicine at Mount Sinai</td>
  <td class="xl74" style="width: 208pt;">0.63132</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl76" style="height: 17.4pt; width: 53pt;">9</td>
  <td class="xl77" style="width: 232pt;"><p><span style="">Ching-Wei
Wang</span></p></td>
  <td class="xl77" style="width: 227pt;">AI Explore&nbsp;</td>
  <td class="xl78" style="width: 208pt;">0.606536</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl72" style="height: 17.4pt; width: 53pt;">10</td>
  <td class="xl70" style="width: 232pt;">Team
  LRDE</td>
  <td class="xl70" style="width: 227pt;">LRDE</td>
  <td class="xl71" style="width: 208pt;">0.529938</td>
 </tr></tbody></table>
 '''
 
- Task 2 : Tumor Burden Estimation
'''html
<tbody><tr style="height: 17.4pt;">
  <td class="xl66" style="height: 17.4pt; width: 34pt;"><b>Rank</b></td>
  <td class="xl67" style="width: 98pt;"><b>Team Name</b></td>
  <td class="xl67" style="width: 271pt;"><b>Affiliation</b></td>
  <td class="xl68" style="width: 53pt;"><b>Score</b></td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl74" style="height: 17.4pt; width: 34pt;">1</td>
  <td class="xl69" style="width: 98pt;">Hyun
  Jung&nbsp;</td>
  <td class="xl69" style="width: 271pt;">Frederick
  National Laboratory for Cancer Research&nbsp;</td>
  <td class="xl72" style="width: 53pt;">0.752826</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl74" style="height: 17.4pt; width: 34pt;">2</td>
  <td class="xl71" style="width: 98pt;">Team
  MIRL-IITM</td>
  <td class="xl71" style="width: 271pt;">Indian
  Institute of Technology Madras</td>
  <td class="xl72" style="width: 53pt;">0.633702</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl73" style="height: 17.4pt; width: 34pt;">3</td>
  <td class="xl71" style="width: 98pt;">Team
  QuIIL</td>
  <td class="xl71" style="width: 271pt;">Sejong
  University</td>
  <td class="xl72" style="width: 53pt;">0.633029</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl73" style="height: 17.4pt; width: 34pt;">4</td>
  <td class="xl71" style="width: 98pt;">Team Damo
  AIC</td>
  <td class="xl71" style="width: 271pt;">Alibaba</td>
  <td class="xl72" style="width: 53pt;">0.619991</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl73" style="height: 17.4pt; width: 34pt;">5</td>
  <td class="xl71" style="width: 98pt;">Team
  COSYPath</td>
  <td class="xl71" style="width: 271pt;">Icahn
  School of Medicine at Mount Sinai</td>
  <td class="xl72" style="width: 53pt;">0.596908</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl73" style="height: 17.4pt; width: 34pt;">6</td>
  <td class="xl71" style="width: 98pt;">Team
  CUHK-Med</td>
  <td class="xl71" style="width: 271pt;">The
  Chinese University of Hong Kong</td>
  <td class="xl72" style="width: 53pt;">0.588317</td>
 </tr>
 <tr style="height: 34.8pt;">
  <td class="xl73" style="height: 34.8pt; width: 34pt;">7</td>
  <td class="xl71" style="width: 98pt;">Team
  DAISYlab@UKE</td>
  <td class="xl71" style="width: 271pt;">University
  Medical Center Hamburg-Eppendorf (UKE)</td>
  <td class="xl72" style="width: 53pt;">0.577394</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl73" style="height: 17.4pt; width: 34pt;">8</td>
  <td class="xl71" style="width: 98pt;">Team
  Sig-IPath</td>
  <td class="xl69" style="width: 271pt;">12sigma
  technology</td>
  <td class="xl72" style="width: 53pt;">0.462489</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl73" style="height: 17.4pt; width: 34pt;">9</td>
  <td class="xl71" style="width: 98pt;">Pingjun
  Chen</td>
  <td class="xl71" style="width: 271pt;">University
  of Florida</td>
  <td class="xl72" style="width: 53pt;">0.43939</td>
 </tr>
 <tr style="height: 17.4pt;">
  <td class="xl73" style="height: 17.4pt; width: 34pt;">10</td>
  <td class="xl71" style="width: 98pt;">Team
  Blackbear</td>
  <td class="xl71" style="width: 271pt;">University
  of Maine, Tianjin Chengjian University</td>
  <td class="xl72" style="width: 53pt;">0.43351</td>
 </tr></tbody></table>
 '''
   

## Strategy

1. Focus on MSI-H detection only (-> how many makers are detected)

![MSI-H](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1850324/bin/jh0212499001.jpg?raw=true)


> Histopathology of medullary carcinoma of the colorectum, a tumor-type characteristic of MSI-H. The malignant cells are large with **abundant pink cytoplasm** and **vesicular nuclei with prominent nucleoli**. Numerous lymphocytes are evident in the malignant epithelium. [2]

2. Focus on tumor masses segmentation only

## References
[1] https://paip2020.grand-challenge.org/

[2] Alexander J, Watanabe T, Wu TT, Rashid A, Li S, Hamilton SR. Histopathological identification of colon cancer with microsatellite instability. Am J Pathol. 2001;158(2):527‐535. doi:10.1016/S0002-9440(10)63994-6

[3] Hou L, Samaras D, Kurc TM, Gao Y, Davis JE, Saltz JH, Patch-based Convolutional Neural Network for Whole Slide Tissue Image Classification. Proc IEEE Comput Soc Conf Comput Vis Pattern Recognit. 2016; 2016:2424-2433. [doi:10.1109/CVPR.2016.266](http://openaccess.thecvf.com/content_cvpr_2016/papers/Hou_Patch-Based_Convolutional_Neural_CVPR_2016_paper.pdf) 


