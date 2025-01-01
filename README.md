
### Project Overview:
![study](studies/LeafDNA/protocols/Studyoverview.png)

---
### Study
#### path to the study folder :  [studies/LeafDNA](studies/LeafDNA)
This project investigates the phyllosphere microbiome of *Arabidopsis thaliana* and its genome. It includes 354 plant samples collected from six wild field sites around Tuebingen, Germany. The samples were gathered over six years (2014-2019), during two seasons each year (spring and fall). For each plant, microbiomes of both epiphytic and endophytic fractions were separated, and DNA was extracted. In total, DNA was collected from 351 endophytic and 352 epiphytic samples. Note: Some plants only have one fraction due to low DNA yield or other experimental challenges. The remaining samples are controls (total = 6), which were used for library preparation for amplicon sequencing.
Metadata for these samples is stored in [studies/LeafDNA/isa.study.xlsx](studies/LeafDNA/isa.study.xlsx).





### Assay1: Amplicon Sequencing
#### path to the assay folder :  [assays/AmpliconData](assays/AmpliconData)
After DNA extraction, amplicon sequencing was performed on the following gene regions:

- **Bacteria**: V3/V4 (BacV3) and V5/V6/V7 (BacV5) regions of the 16S rRNA gene
- **Fungi**: ITS1 (Ftrad) and ITS2 (FITS2) regions
- **Oomycetes**: ITS1 (Otrad) and ITS2 (OITS2) regions
- **Eukaryotes**: V4/V5 (PrV4) and V9 (PrV9) regions of the 18S rRNA gene

In total, 4,368 libraries (samples) were prepared. These libraries were sequenced over 11 runs using the Illumina MiSeq platform. For each run, forward, reverse, and index FASTQ files were generated.

The sequences were multiplexed during sequencing, and demultiplexing can be done using the barcode file located in each run folder. Please note that only reverse barcodes are available for demultiplexing and/or creating contigs. The associated metadata is stored in [assays/AmpliconData/isa.assay.xlsx](assays/AmpliconData/isa.assay.xlsx).

---

### Assay2: Whole Genome Sequencing
#### path to the assay folder :  [assays/WholeGenomeData](assays/WholeGenomeData)
Whole genome sequencing was performed on 103 endophytic DNA samples using the Illumina MiSeq platform (2 x 150bp reads). For each sample, four FASTQ files were generated:
- `L001_Forward`
- `L001_Reverse`
- `L002_Forward`
- `L002_Reverse`

Here, L001 and L002 represent different lanes of the sequencing flow cell. In rare cases of production issues with the flow cell, these lanes may have different quality scores. Therefore, the data is provided separately for each lane.  The associated metadata is stored in
 [assays/WholeGenomeData/isa.assay.xlsx](assays/WholeGenomeData/isa.assay.xlsx).

---

### Workflow for Amplicon Sequencing Data:

[workflows/Ampliconseq](workflows/Ampliconseq) \
Sequences from the Bacteria V5/V6/V7 (BacV5), Fungal ITS2 (FITS2), and Eukaryotic V9 (PrV9) samples were processed using the Mothur pipeline, and OTU (Operational Taxonomic Unit) tables were generated.

---

### Workflow for Whole Genome Sequencing Data:

[workflows/wholegenomeseq](workflows/wholegenomeseq) \
An example pipeline to generate single nucleotide polymorphisms (SNPs) from whole genome sequencing data is available.

---

### Citing This Dataset And Related Publication
Citing our work helps support the ongoing development and maintenance of this dataset. If you use this dataset in your research, please cite it using this DOI: [https://doi.org/10.57754/FDAT.61ckt-vm178] 

Additionally, the following publications have utilized this dataset:

- **Mahmoudi *et al.,* 2024**. *Microbial communities living inside plant leaves or on the leaf surface are differently shaped by environmental cues*., Pages. DOI: [https://doi.org/10.1093/ismeco/ycae103]

- **Mahmoudi *et al.,* 2024**. *Biotic interactions shape infection outcomes in Arabidopsis*., Pages. DOI: [https://doi.org/10.1101/2024.10.25.620230]

- **Höhn *et al.,* 2024**. *Strong pairwise interactions do not drive interactions in a plant leaf associated microbial community*., Pages. DOI: [https://doi.org/10.1093/ismeco/ycae117]

- **Gómez-Pérez *et al.,* 2022**. *Proteins released into the plant apoplast by the obligate parasitic protist Albugo selectively repress phyllosphere-associated bacteria*., Pages. DOI: [https://doi.org/10.1111/nph.18995]

- **Agler *et al.,* 2016**. *Microbial Hub Taxa Link Host and Abiotic Factors to Plant Microbiome Variation*., Pages. DOI: [https://doi.org/10.1371/journal.pbio.1002352]

---
### Contact us 

[Kemen lab](https://uni-tuebingen.de/en/fakultaeten/mathematisch-naturwissenschaftliche-fakultaet/fachbereiche/zentren/zentrum-fuer-molekularbiologie-der-pflanzen/research/research-groups/microbial-interactions/people/)


Administrative \
Eric Kemen (eric.kemen@zmbp.uni-tuebingen.de)

Technical \
Maryam Mahmoudi (https://maryambio.github.io) \
Hamed Jalali (hamed.jalali@uni-tuebingen.de) 

University of Tuebingen Germany \
IMIT/ZMBP \
Mikrobielle Interaktionen \
Auf der Morgenstelle 32 \
D-72076 Tübingen




