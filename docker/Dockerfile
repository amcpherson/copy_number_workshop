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

