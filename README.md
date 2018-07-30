# ELIXIR Marine Metagenomics Implementation Plan
A web-service supporting ITS1-based survey of marine communities.

## BioMaS galaxy wrapper
BioMaS: a modular pipeline for Bioinformatic analysis of Metagenomic AmpliconS (Galaxy version).

### Dependencies

1. xvfb-run has to be installed on your instance (and on each Worker Node if using a cluster).
   to run the ETE toolkit: http://etetoolkit.org/docs/latest/tutorial/tutorial_webplugin.html

Ubuntu 16.04
```
# apt-get install libsm6 libxt6 libxrender1
# apt-get install xvbf
```

CentOS 7
```
# yum install libXext libSM libXrender
# yum install xorg-x11-server-Xvfb
```

2. Install usearch on each Cluster Worker Node, copying it in /usr/bin

Troubleshooting
---------------
1. fastqc fix: type this command inside the conda environment
```
<conda_prefix>/bin/conda install -y --name mulled-v1-52d3dd165352f3c2fa0613c44045f9f49653b44c9906c50bba2a986824f9e457 openjdk --channel conda-forge
```
