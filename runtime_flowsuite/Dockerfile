FROM tercen/runtime-r40:4.0.4-1

RUN apt-get update
RUN apt-get install -y libglpk-dev
RUN apt-get install -y r-cran-rcppparallel
RUN apt-get install -y r-cran-rcpparmadillo
RUN apt-get install -y r-cran-igraph

RUN R -e "BiocManager::install('MetaCyto')"
RUN R -e "remotes::install_github('ghar1821/TrackSOM')"
RUN R -e "remotes::install_github('tercen/tim')"
RUN R -e "remotes::install_github('tercen/teRcenHttp')"
RUN R -e "remotes::install_github('tercen/mtercen')"
#RUN R -e "remotes::install_github('tercen/tercenApi', ref = '7f1274676d90681341833c289688e80f45c2638f')"
RUN R -e "remotes::install_github('tercen/teRcen', ref='0.11.3')"

RUN R -e "BiocManager::install('openCyto')"
RUN R -e "BiocManager::install('diffcyt')"
