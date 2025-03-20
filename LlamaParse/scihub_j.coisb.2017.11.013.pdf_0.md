# Identifying noise sources governing cell-to-cell variability

# Simon Mitchell and Alexander Hoffmann

# Abstract

Phenotypic differences often occur even in clonal cell populations. Many potential sources of such variation have been identified, from biophysical rate variance intrinsic to all chemical processes to asymmetric division of molecular components extrinsic to any particular signaling pathway: Identifying the sources of phenotypic variation and quantifying their contributions to cell fate variation is not possible without accurate single cell data. By combining such data with mathematical models of potential noise sources it is possible to characterize the impact of varying levels of each noise source and identify which sources of variation best explain the experimental observations. The mathematical framework of information theory provides metrics of the impact of noise on the reliability of a cell to sense its environment: While the presence of noise in a single cellular system reduces the reliability of signal transduction, its impact on a population of varied single cells remains unclear.

Numerous theoretical and experimental studies have addressed the sources and physiological consequence of this variability. A useful distinction is whether the source of the variability is intrinsic or extrinsic to the regulatory system and timescale being considered: That distinction has indeed important implications to both the biology and our study of it. As intrinsic molecular variability reflects thermodynamic noise of molecular interactions within the regulatory network, modeling it requires stochastic mathematical representation (e.g., Gillespie formalisms) and may limit the predictability of biological phenotypes and reliability of signal transduction (Figure IA). In contrast, extrinsic noise reflects distinct starting conditions (initial concentrations and/or kinetic rate constants) of the molecular networks of individual cells within the population, distinct time-dependent inputs (changes in the environment) to the system. In principle, biological outcomes that are only subject to extrinsic noise can be predicted and modeled with deterministic mathematical formalisms (e.g., ordinary differential equations) so long as the starting conditions and inputs to the system are known. Further, information loss through extrinsic noise can be mitigated through Dynamical Signaling Code. By leveraging information contained in time trajectories, the reliability of signaling is not diminished by extrinsic noise.

# Keywords

Single-cell; Noise; Variability; Computational modeling; Signal transduction;

# Introduction

Cells must reliably sense their environment in order to behave and respond appropriately: Sources of information in the environment are highly varied and can include nutrient availability, cytokine and chemokine levels, pathogens and combinations thereof: Sensing the cellular environment typically involves receptor activation and transduction of receptor state information through signaling networks resulting in an appropriate response. Such responses can take the form of gene expression.

# Addresses

Institute for Quantitative and Computational Biosciences, Department of Microbiology, Immunology, and Molecular Genetics, University of California Los Angeles, CA 90095, USA

Corresponding author: Hoffmann, Alexander (ahoffmann@ucla.edu)

# Current Opinion in Systems Biology 2018, 8.39-45

This review comes from themed issue on Special Section: Single cell and systems biology (2018)

Edited by Frank J. Bruggeman and Peter Swain

Available online December 2017

https://doi.org/10.1016/j.coisb.2017.11.013

2452-3100/0 2017 Elsevier Ltd. All rights reserved.