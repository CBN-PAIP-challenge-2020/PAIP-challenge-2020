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

## Strategy

1. Focus on MSI-H detection only (-> how many makers are detected)
2. Focus on tumor masses segmentation only

