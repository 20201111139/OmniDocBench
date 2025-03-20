# ScienceDirect  

ELSEVIER  

# Identifying noise sources governing cell-to-cell variability Simon Mitchell and Alexander Hoffmann  

# Abstract  

Phenotypicdifferencesoften occureven in clonal cellpopulations.Manypotential sourcesofsuchvariationhavebeen identified,frombiophysical ratevarianceintrinsictoall chemicalprocesses toasymmetricdivision ofmolecularcomponents extrinsic to any particular signaling pathway. ldentifying the sources of phenotypicvariation and quantifying their contributionstocellfatevariationisnotpossiblewithoutaccurate singlecelldata.Bycombiningsuchdatawithmathematical modelsofpotentialnoisesourcesitispossibletocharacterize theimpactofvaryinglevelsofeachnoisesourceandidentify whichsourcesofvariationbestexplainthe experimental observations.Themathematical frameworkof information theory providesmetricsof theimpactofnoiseonthereliabilityofacell tosenseitsenvironment.While thepresenceofnoiseina singlecellularsystemreducesthereliabilityofsignal transductionitsimpactonapopulationofvariedsinglecellsremains unclear.  

# Addresses  

InstituteforQuantitativeand Computational Biosciences,Department of Microbiology,Immunology,and Molecular Genetics,University of California,LosAngeles,CA90095,USA  

Corresponding author:Hoffmann,Alexander(ahoffmann@ucla.edu)  

# CurrentOpinion inSystems Biology2018,8:39-45  

This review comes from a themed issue on Special Section:Single cell and systemsbiology(2018)  

Edited byFrankJ.Bruggeman and PeterSwain  

Availableonline6December2017  

https://doi.org/10.1016/j.coisb.2017.11.013  

2452-3100/2017ElsevierLtd.Allrightsreserved  

# Keywords  

Single-cell,Noise,Variability,Computational modeling, Signal transduction.  

# Introduction  

Cellsmust reliably sense their environment in order to behave and respond appropriately. Sources of information in the environment are highly varied and can include nutrient availability, cytokine and chemokine levels, pathogens and combinations thereof. Sensing the cellular environment typically involves receptor activation and transduction of receptor state information through a signaling network resulting in an appropriate response. Such responses can take the form of gene expression[1],or cell fate decisions such as differentiation [2], division and death  $[3^{\circ}]$  .Mechanistic computational models of signalingnetworks arevaluable tools to explain how a cell canrespond to environmental cues with stimulus specific gene expression [4], differentiation [5,6],division[7] and death[3,8].  

However,single cell studieshave revealed a high degree of variability in the responses of genetically identical cells grown and treated in identical conditions. Numerous theoretical and experimental studies have addressed the sources and physiological consequence of this variability [9-11].A useful distinction is whether the source of the variability is intrinsic or extrinsic to the regulatory system and timescale being considered. That distinction has indeed important implications to both the biology and our study of it. As intrinsic molecular variability refects thermodynamic noise of molecular interactions within the regulatory network, modeling, it requires stochastic mathematical representation (e.g. Gillespie formalisms), and may limit the predictability of biological phenotypes, or reliability of signal transduction (Figure 1A). In contrast, extrinsic noise reflects distinct starting conditions (initial concentrations and/ orkineticrate constants)of themolecularnetworks of individual cells within the population, or distinct timedependent inputs (changes in the environment) to the system [12,13].In principle,biological outcomes that are only subject to extrinsic noise can be predicted and modeledwithdeterministicmathematicalformalisms (e.g. ordinary differential equations) so long as the startingconditions and inputsto the system areknown. Further,information loss through extrinsic noise can be mitigated through a Dynamical Signaling Code [14,15]. By leveraging information contained in time trajectories, the reliability of signaling is not diminished by extrinsic noise (Figure 1B and C) [16,17].  

In a seminal study, an engineered bacterial system was developed to quantify the contribution of extrinsic and intrinsic noise sources to the expression of identical duplicate reporter genes [18]. However, such elegant engineering of signaling systems is notpossible in many biological contexts such as the immune system[19.20]. For natural biological systems computational models can provideatooltoelucidatehowdifferentsourcesof variability can result in distinct phenotypes.  

Herewewill describehow recent advances in single-cell imaging, combined with computational models enable  