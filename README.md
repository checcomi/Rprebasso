
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Rprebasso - R library for PRELES + CROBAS + YASSO model

<!-- badges: start -->

<!-- badges: end -->

Rprebasso is a forest growth and ecosystem carbon balance model. In
PREBASSO three different models PRELES (PREdict Light-use efficiency,
Evapotranspiration and Soil water), CROBAS (Tree growth and CROwn BASe
from carbon balance), and YASSO (Yet Another Simulator of Soil Organic
matter) are coupled together in order to predict the growth and carbon
balance of the forest ecosystem. CROBAS provides estimates of LAI (Leaf
Area Index) that is used in PRELES to compute gross primary production.
GPP is then used by CROBAS to estimate forest growth. The stand
structural variables and the biomass components of the forest are
updated. Meanwhile, CROBAS estimates the litter production that is the
input of YASSO.

## Installation

You can install the the development version from
[GitHub](https://github.com/ForModLabUHel/Rprebasso) with:

``` r
# install.packages("devtools")
devtools::install_github("ForModLabUHel/Rprebasso")
```

## References

Mäkelä, Annikki. 1997. “A Carbon Balance Model of Growth and
Self-Pruning in Trees Based on Structural Relationships.” Forest Science
43 (1): 7–24. <https://doi.org/10.1093/forestscience/43.1.7>.

Mäkelä, Annikki, Minna Pulkkinen, Pasi Kolari, Fredrik Lagergren, Paul
Berbigier, Anders Lindroth, Denis Loustau, Eero Nikinmaa, Timo Vesala,
and Pertti Hari. 2008. “Developing an Empirical Model of Stand GPP with
the LUE Approach: Analysis of Eddy Covariance Data at Five Contrasting
Conifer Sites in Europe.” Global Change Biology 14 (1): 92–108.
<https://doi.org/10.1111/j.1365-2486.2007.01463.x>.

Minunno, F., M. Peltoniemi, S. Launiainen, M. Aurela, A. Lindroth, A.
Lohila, I. Mammarella, K. Minkkinen, and A. Mäkelä. 2016. “Calibration
and Validation of a Semi-Empirical Flux Ecosystem Model for Coniferous
Forests in the Boreal Region.” Ecological Modelling 341.
<https://doi.org/10.1016/j.ecolmodel.2016.09.020>.

Minunno, Francesco, Mikko Peltoniemi, Sanna Härkönen, Tuomo Kalliokoski,
Harri Makinen, and Annikki Mäkelä. 2019. “Bayesian Calibration of a
Carbon Balance Model PREBAS Using Data from Permanent Growth Experiments
and National Forest Inventory.” Forest Ecology and Management 440 (May):
208–57. <https://doi.org/10.1016/J.FORECO.2019.02.041>.

Peltoniemi, Mikko, Minna Pulkkinen, Mika Aurela, Jukka Pumpanen, Pasi
Kolari, and Annikki Mäkelä. 2015. “A Semi-Empirical Model of
Boreal-Forest Gross Primary Production, Evapotranspiration, and Soil
Water — Calibration and Sensitivity Analysis.” Boreal Environment
Research 20 (2): 151–71.
<https://helda.helsinki.fi/handle/10138/228031>.

Tian, X., Minunno, F., Cao, T., Kalliokoski, T., Mäkelä, A. 2020.
“Extending the range of applicability of the semi‐empirical ecosystem
flux model PRELES for varying forest types and climate.” Global Change
Biology 26: 2923–2943.https://doi.org/10.1111/gcb.14992

## Acknowledgements:

The model and package developments were supported by:

The Horizon 2020 Research and innovation framework program (Forest
Carbon Flux and Storage Mapping Service, proposal \#821860)

The Strategic Research Council at the Academy of Finland (IBC-CARBON,
decision. \#312635)

…

PREBAS has been initially developed, calibrated and tested for the
boreal forest ecosystems, while in the project [Forest Carbon Flux and
Storage Mapping Service](https://www.forestflux.eu/) we are extending
the model application to temperate, Mediterranean and sub-tropical
ecosystems.

This work used eddy covariance data acquired and shared by the FLUXNET
community, including these networks: AmeriFlux, AfriFlux, AsiaFlux,
CarboAfrica, CarboEuropeIP, CarboItaly, CarboMont, ChinaFlux,
Fluxnet-Canada, GreenGrass, ICOS, KoFlux, LBA, NECC, OzFlux-TERN,
TCOS-Siberia and USCCC. The ERA-Interim reanalysis data were provided by
the ECMWF and processed by the LSCE. The FLUXNET eddy covariance data
processing and harmonization were carried out by the European Fluxes
Database Cluster, AmeriFlux Management Project and Fluxdata project of
FLUXNET, with the support of the CDIAC and ICOS Ecosystem Thematic
Centre, and the OzFlux, ChinaFlux and AsiaFlux offices.

Model performance has been evaluated for stands in Baden-Württemberg of
Germany. Results produced using map and other data types kindly provided
by the Department for Forest Management and Forest Geoinformation of the
State Forest Administration of the German Federal State
Baden-Württemberg in 2021
(<https://rp.baden-wuerttemberg.de/rpf/abt8/ref85/>). We further thank
the communities located in the German Federal State Baden-Württemberg
that kindly allowed the utilization of their forest management data that
were provided via the Department for Forest Management and Forest
Geoinformation: Ettenheim, Zell a.H., Bad Peterstal-Griesbach,
Friesenheim, Kappel-Grafenhausen, Lauf, Neuried, Oberharmersbach,
Sasbach.
