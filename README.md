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
- **[Top Ranked Team's Presentation Material](https://drive.google.com/file/d/1NWJdZJFHajHfod5fgO7WnoRqYuQGN_tp/view)**
- Task 1 : Tumor Segmentation

|__Rank__|__Team Name__|__Affiliation__|__Score__|__Model__|__Patch-Wise__|__Pixel_Wise__|__Ensemble__|
|:------:|:-----------:|:-------------:|:-------:|:-------:|:------------:|:------------:|:----------:|
|1       |Hyun Jung    |Frederick National Laboratory for Cancer Research|0.788987|EfficientNet-B4, UNet++|O|O|O|
|2       |Team Sen	    |Sichuan University|0.777215|SE-Resnext101, U-Net|O|O|O|
|3       |Team MIRL-IITM	|Indian Institute of Technology Madras	|0.750333|DensNet-121, InceptionResNetV2, DeeplabV3plus| |O|O|
|4       |Team Damo AIC	|Alibaba - alicloud 	|0.671778|Resnet101, U-Net| |O|O|
|5       |Team QuIIL	|Sejong University	|0.665227|Densely connected convolutional block, U-net| | |O|
|6       |Team CUHK-Med	|The Chinese University of Hong Kong	|0.662454|msYI-Net(ResNet18-U-Net)| |O|O|
|7       |Team DAISYlab@UKE	|University Medical Center Hamburg-Eppendorf (UKE)	|0.65962|SegNet| |O|O|
|8       |Team COSYPath	|Icahn School of Medicine at Mount Sinai	|0.63132|-|-|-|-|
|9       |Ching-Wei Wang |AI Explore 	|0.606536|Custom VGG16(Segmentation)| |O| |
|10      |Team LRDE	|LRDE	|0.529938|Unet512, Unet2048| |O| |

 
- Task 2 : Tumor Burden Estimation

|__Rank__|__Team Name__|__Affiliation__|__Score__|__Model__|__Patch-Wise__|__Pixel_Wise__|__Ensemble__|
|:------:|:-----------:|:-------------:|:-------:|:-------:|:------------:|:------------:|:----------:|
|1|Hyun Jung|Frederick National Laboratory for Cancer Research 	|0.752826|EfficientNet-B4, UNet++|O|O|O|
|2|Team MIRL-IITM	|Indian Institute of Technology Madras	|0.633702|SE-Resnext101, U-Net|O|O|O|
|3|Team QuIIL	|Sejong University	|0.633029|DensNet-121, InceptionResNetV2, DeeplabV3plus| |O|O|
|4|Team Damo AIC	|Alibaba	|0.619991|Resnet101, U-Net| |O|O|
|5|Team COSYPath	|Icahn School of Medicine at Mount Sinai	|0.596908|-|-|-|-|
|6|Team CUHK-Med	|The Chinese University of Hong Kong	|0.588317|msYI-Net(ResNet18-U-Net)| |O|O|
|7|Team DAISYlab@UKE	|University Medical Center Hamburg-Eppendorf (UKE)	|0.577394|SegNet| |O|O|
|8|Team Sig-IPath	|12sigma technology	|0.462489|-|-|-|-|
|9|Pingjun Chen	|University of Florida	|0.43939|-|-|-|-|
|10|Team Blackbear	|University of Maine, Tianjin Chengjian University	|0.43351

results source : [url](https://drive.google.com/file/d/1ierVsP82cPBGsi5djqoEHtRmcVF1lDe1/view)

1. Focus on MSI-H detection only (-> how many makers are detected)

![MSI-H](https://github.com/gj21kr/PAIP-challenge-2020/blob/master/references/jh0212499001.jpg?raw=true)

> Histopathology of medullary carcinoma of the colorectum, a tumor-type characteristic of MSI-H. The malignant cells are large with abundant pink cytoplasm and vesicular nuclei with prominent nucleoli. Numerous lymphocytes are evident in the malignant epithelium.

![](https://media.springernature.com/full/springer-static/image/art%3A10.1186%2Fs41241-017-0020-1/MediaObjects/41241_2017_20_Fig1_HTML.gif?as=webp)

> Three major pathways leading to colorectal cancers. (1) Conventional adenoma-carcinoma sequence with oncogene (e.g. KRAS) activation and tumor suppressor (e.g. APC, SMAD4 and TP53) inactivation, resulting in microsatellite stable (MSS) cancers; (2) Microsatellite instability (MSI) pathway with mismatch repair (MMR) protein deficiency in patients with Lynch syndrome, resulting in MSI-high (MSI-H) cancers; (3) Serrated pathway with CpG island methylation phenotype, resulting in either MSI-H cancers if methylation occurs in MLH1 promoter or MSS cancers if methylation occurs in tumor suppressor genes. HGD: high-grade dysplasia; LGD: low-grade dysplasia; SSA: sessile serrated adenoma [2]

> [Reference Publication[4]](https://www.nature.com/articles/s41591-019-0462-y)

> [More Details](https://docs.google.com/presentation/d/1aY4T2eI27-ScpZvG5AghM0yntjFSYMPdRwOtR5nqp4Y/edit?usp=sharing)

2. Focus on tumor masses segmentation only

> [Keynote Medical Summary](https://drive.google.com/file/d/1b-ZcBFJBYG8knyZ4VvBGXIijApxJLgrA/view)
> [Keynote Multi-Scale Multi-Encoder](https://drive.google.com/file/d/1mFhivlYfGEjM5CTbX7qHlDyXHQ3JxaP3/view)

## References
[1] https://paip2020.grand-challenge.org/

[2] Gonzalez, R.S., Washington, K. & Shi, C. Current applications of molecular pathology in colorectal carcinoma. Appl Cancer Res 37, 13 (2017). [doi:10.1186/s41241-017-0020-1](https://doi.org/10.1186/s41241-017-0020-1)

[3] Hou L, Samaras D, Kurc TM, Gao Y, Davis JE, Saltz JH, Patch-based Convolutional Neural Network for Whole Slide Tissue Image Classification. Proc IEEE Comput Soc Conf Comput Vis Pattern Recognit. 2016; 2016:2424-2433. [doi:10.1109/CVPR.2016.266](http://openaccess.thecvf.com/content_cvpr_2016/papers/Hou_Patch-Based_Convolutional_Neural_CVPR_2016_paper.pdf) 

[4] Kather, J.N., Pearson, A.T., Halama, N. et al. Deep learning can predict microsatellite instability directly from histology in gastrointestinal cancer. Nat Med 25, 1054–1056 (2019). [doi:10.1038/s41591-019-0462-y](https://doi.org/10.1038/s41591-019-0462-y)
