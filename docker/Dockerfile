FROM rocker/tidyverse:4.4.1

RUN apt-get update -y
RUN apt-get install libxt-dev libmagick++-dev libglpk-dev -y
RUN install2.r --error bookdown
RUN install2.r --error ggExtra
RUN install2.r --error factoextra
RUN install2.r --error igraph
RUN R -e 'BiocManager::install("bluster")'
RUN install2.r --error ggbeeswarm
RUN install2.r --error umap
RUN R -e 'BiocManager::install("Homo.sapiens")'
RUN R -e 'BiocManager::install("ComplexHeatmap")'
RUN R -e 'BiocManager::install("ggtree")'
RUN install2.r --error phytools
RUN install2.r --error vcfR
RUN R -e 'BiocManager::install("BSgenome.Hsapiens.UCSC.hg19")'
RUN R -e 'BiocManager::install("MutationalPatterns")'
RUN R -e 'devtools::install_github("shahcompbio/signals")'
RUN install2.r --error VGAM
RUN R -e 'BiocManager::install("SingleCellExperiment")'
RUN apt-get install jags
RUN R -e 'BiocManager::install("infercnv")'
RUN install2.r --error Seurat

