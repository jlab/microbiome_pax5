## Computational Analysis for "An intact gut microbiome protects genetically predisposed mice against leukemia."

Carolina Vicente-Dueñas, Stefan Janssen, Marina Oldenburg, Franziska Auer, Inés González-Herrero, Ana Casado-García, Marta Isidro-Hernández, Javier Raboso-Gallego, Philipp Westhoff, Aleksandra A. Pandyra, Daniel Hein, Katharina L. Gössling, Diego Alonso-López, Javier De Las Rivas, Sanil Bhatia, Francisco Javier García Criado, María Begoña García Cenador, Andreas P. M. Weber, Karl Köhrer, Julia Hauer, Ute Fischer, Isidro Sánchez-García, Arndt Borkhardt

#### Abstract
The majority of childhood leukemias are precursor B cell-acute lymphoblastic leukemias (pB-ALL) caused by a combination of prenatal genetic predispositions and oncogenic events occurring after birth. Although genetic predispositions are frequent in children (>1-5%), fewer than 1% of genetically predisposed carriers will develop pB-ALL. While infectious stimuli are believed to play a major role in leukemogenesis, the critical determinants are not well defined. Here, employing murine models of pB-ALL, we show that microbiome disturbances incurred by antibiotic treatment early in life were sufficient to induce leukemia in genetically predisposed mice even in the absence of infectious stimuli and independent of T-cells. Using V4 and full-length 16S rRNA sequencing of a series of fecal samples, we found that genetic predisposition to pB-ALL (Pax5 heterozygosity or ETV6-RUNX1 fusion) shaped a distinct gut microbiome. Machine learning accurately (96.8%) predicted genetic predisposition using 40 of 3,983 amplicon sequence variants (ASVs) as proxies for bacterial species. Transplantation of either wild type (WT) or Pax5+/- hematopoietic bone marrow cells into WT recipient mice revealed that the microbiome is shaped and determined in a donor-genotype-specific manner. Gas chromatography-mass spectrometric (GC-MS) analyses of sera from WT and Pax5+/- mice demonstrated the presence of a genotype-specific distinct metabolomic profile. Taken together, our data indicate that it is a lack of commensal microbiota rather than the presence of specific bacteria that promotes leukemia in genetically predisposed mice. Future large-scale longitudinal studies are required to determine whether targeted microbiome modification in children predisposed to pB-ALL could become a successful prevention strategy.   

#### Instructions
You will find our analysis [jupyter notebook](https://jupyter.org/) in the sub-directory 4Cohorts entitled [pax5_cohousing_abx_bmt.ipynb](4Cohorts/pax5_cohousing_abx_bmt.ipynb).

Raw sequence data can be retrieved from [Qiita](https://qiita.ucsd.edu/), study IDs 11758, 11953, 12981, 13189. For your convenience, the pre-processing results (i.e. feature-tables) are contained in 4Cohorts/FromQiita together with preparation and sample metadata information.
You might alternatively download sequences from ENA: ERP117561, ERP117668, ERP122650, ERP122653.

There is a bunch of additional software necessary to actually re-compute each and every analysis step. Most notabely
  - [qiime2](qiime2.org/) (version 2020.2)
  - [ggmap](https://github.com/sjanssen2/ggmap) (a collection of custom build helper scripts)
Function in ggmap will call several conda environments, whose build recipies are contained in ggmap sources.

Shoot your questions to stefan.janssen@computational.bio.uni-giessen.de

#### Figures
In principle, figures are generated via the notebook. However, some of the figures in the manuscript have manually been polished via Inkscape or other graphic software. Those manually touched versions are stored in the sub-directory [4Cohorts/Figures](4Cohorts/Figures) as \*.svg files.
