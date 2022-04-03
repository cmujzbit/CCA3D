# Base jupyter image.
ARG BASE_CONTAINER=jupyter/datascience-notebook
FROM $BASE_CONTAINER

# TODO : Add other maintainers.
LABEL maintainer="Cezary Turek <cezary.turek@gmail.com>"

# INFO : Use if Linux libs are extended.
#USER root
#USER $NB_UID

# Install R packages.
RUN R --vanilla -e "install.packages(c('PMA', 'readxl', 'CCA'), repos='http://cran.us.r-project.org')"
